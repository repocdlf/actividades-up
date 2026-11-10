# actividades-up
Actividades de BB de UP

## instalacion de draw.io con powershell
winget install --id JGraph.Draw --scope user --accept-source-agreements --accept-package-agreements

## agregar al path del usuario
$drawioDir="$env:LOCALAPPDATA\Programs\draw.io";$drawioDir;if(-not(([Environment]::GetEnvironmentVariable('Path','User')-split';')-contains$drawioDir)){[Environment]::SetEnvironmentVariable('Path',[Environment]::GetEnvironmentVariable('Path','User')+";$drawioDir",'User')};([Environment]::GetEnvironmentVariable('Path','User')-split';')

## validar version instalada
draw.io --version

