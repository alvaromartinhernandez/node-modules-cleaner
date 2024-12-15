# node-modules-cleaner

This PowerShell script searches for and deletes all `node_modules` folders in a specified path, helping to free up disk space.

## Usage

1. Run the `delete_node_modules.ps1` script in PowerShell.
2. Enter the path where you want to search for the `node_modules` folders. If you leave the field empty, `C:` will be used by default (this can be slow).
3. The script will ask you if you want to show the detail of each folder processed. Answer `s` for yes or `n` for no.
4. The script will look for all `node_modules` folders in the specified path and calculate the total space occupied by them.
5. You will be asked if you want to delete all the `node_modules` folders found. Answer `s` for yes or `n` for no.

## Example

````powershell
PS C:\> .\delete_node_modules.ps1
Enter the path to search for the node_modules folders (leave empty to use 'C:\', this can be slow):
Do you want to show the detail of each processed folder (y/n): s
Folder: C:__project_node_modules - Size: 150 MB
Folder: C:other_project_modules - Size: 200 MB
Total space occupied by node_modules: 0.34 GB
Do you want to delete all node_modules folders found (y/n): s
Deleted folder: C:\project\node_modules
Deleted folder: C:other_project_modules
All node_modules folders have been deleted.
````


## Warning
Note that this script will permanently delete the node_modules folders found. Make sure you don't need any of them before proceeding with the deletion.



# node-modules-cleaner (ES)

Este script de PowerShell busca y elimina todas las carpetas `node_modules` en una ruta especificada, ayudando a liberar espacio en disco.

## Uso

1. Ejecuta el script `delete_node_modules.ps1` en PowerShell.
2. Introduce la ruta donde deseas buscar las carpetas `node_modules`. Si dejas el campo vacío, se usará `C:\` por defecto (esto puede ser lento).
3. El script te preguntará si deseas mostrar el detalle de cada carpeta procesada. Responde `s` para sí o `n` para no.
4. El script buscará todas las carpetas `node_modules` en la ruta especificada y calculará el espacio total ocupado por ellas.
5. Se te preguntará si deseas eliminar todas las carpetas `node_modules` encontradas. Responde `s` para sí o `n` para no.

## Ejemplo

```powershell
PS C:\> .\delete_node_modules.ps1
Introduce la ruta donde buscar las carpetas node_modules (deja vacío para usar 'C:\', esto puede ser lento):
¿Quieres mostrar el detalle de cada carpeta procesada? (s/n): s
Carpeta: C:\proyecto\node_modules - Tamaño: 150 MB
Carpeta: C:\otro_proyecto\node_modules - Tamaño: 200 MB
Espacio total ocupado por node_modules: 0.34 GB
¿Quieres borrar todas las carpetas node_modules encontradas? (s/n): s
Carpeta eliminada: C:\proyecto\node_modules
Carpeta eliminada: C:\otro_proyecto\node_modules
Todas las carpetas node_modules han sido eliminadas.
```

## Advertencia
Ten en cuenta que este script eliminará permanentemente las carpetas node_modules encontradas. Asegúrate de que no necesitas ninguna de ellas antes de proceder con la eliminación.

