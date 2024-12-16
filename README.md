# node-modules-cleaner

This PowerShell script helps you search for and optionally delete all `node_modules` folders in a specified path. It's a useful tool for freeing up disk space, especially for developers who manage multiple projects.

## Features
- **Multilingual support**: The script automatically adjusts to your system language (`en` or `es`). Defaults to English for unsupported languages.
- **Customizable scan path**: Choose the directory to scan, with `C:\` as the default path.
- **Log details**: Optionally display the size and location of each `node_modules` folder found.
- **Disk space calculation**: View the total space occupied by all `node_modules` folders.
- **Safe deletion**: Confirm before deleting the folders, with clear feedback during the process.

## Usage

1. Run the script `delete_node_modules.ps1` in PowerShell.
2. Enter the path where you want to search for `node_modules` folders. If you leave the field empty, the script will use `C:\` as the default (this might be slow).
3. The script will prompt you to display the details of each folder found. Answer `y` (yes) or `n` (no).
4. It will search for all `node_modules` folders in the specified path and calculate their total disk usage.
5. You will be asked if you want to delete all the `node_modules` folders found. Answer `y` (yes) or `n` (no).

### Example
```powershell
PS C:\> .\delete_node_modules.ps1
Enter the path to search for 'node_modules' folders (leave empty to use 'C:\', this can be slow):
C:\projects
Do you want to show the details of each processed folder? (y/n): y
Folder: C:\projects\project1\node_modules - Size: 150 MB
Folder: C:\projects\project2\node_modules - Size: 200 MB
Total space occupied by 'node_modules': 0.34 GB
Do you want to delete all 'node_modules' folders found? (y/n): y
Deleted folder: C:\projects\project1\node_modules
Deleted folder: C:\projects\project2\node_modules
All 'node_modules' folders have been deleted.
````


## Warning
- **Permanent Deletion**: This script will permanently delete all node_modules folders found. Ensure you don’t need any of them before proceeding.
- **Performance Tip**: Scanning large directories like C:\ can take significant time. Use a shorter path to speed up the process.


# node-modules-cleaner (ES)

Este script de PowerShell te ayuda a buscar y, opcionalmente, eliminar todas las carpetas `node_modules` en una ruta especificada. Es útil para liberar espacio en disco, especialmente para desarrolladores con múltiples proyectos.

### Características
- **Soporte multilingüe**: El script se ajusta automáticamente al idioma del sistema (`en` o `es`). Por defecto, utiliza inglés si el idioma no es compatible.
- **Ruta de búsqueda personalizada**: Escoge el directorio a analizar, con `C:\` como ruta predeterminada.
- **Detalles del registro**: Muestra opcionalmente el tamaño y la ubicación de cada carpeta `node_modules` encontrada.
- **Cálculo del espacio en disco**: Consulta el espacio total ocupado por todas las carpetas `node_modules`.
- **Eliminación segura**: Confirma antes de borrar las carpetas y ofrece un seguimiento claro durante el proceso.

### Uso
- Ejecuta el script `delete_node_modules.ps1` en PowerShell.
- Introduce la ruta donde deseas buscar las carpetas `node_modules`. Si dejas el campo vacío, se usará `C:\` como predeterminado (esto puede ser lento).
- El script te pedirá mostrar los detalles de cada carpeta encontrada. Responde `s` (sí) o `n` (no).
- Buscará todas las carpetas `node_modules` en la ruta especificada y calculará su uso total de disco.
- Se te preguntará si deseas eliminar todas las carpetas `node_modules` encontradas. Responde `s` (sí) o `n` (no).

### Ejemplo

```powershellPS C:\> .\delete_node_modules.ps1
Introduce la ruta donde buscar carpetas 'node_modules' (deja vacío para usar 'C:\', esto puede ser lento):
C:\proyectos
¿Quieres mostrar el detalle de cada carpeta encontrada? (s/n): s
Carpeta: C:\proyectos\proyecto1\node_modules - Tamaño: 150 MB
Carpeta: C:\proyectos\proyecto2\node_modules - Tamaño: 200 MB
Espacio total ocupado por 'node_modules': 0.34 GB
¿Quieres borrar todas las carpetas 'node_modules' encontradas? (s/n): s
Carpeta eliminada: C:\proyectos\proyecto1\node_modules
Carpeta eliminada: C:\proyectos\proyecto2\node_modules
Todas las carpetas 'node_modules' han sido eliminadas.
````

### Advertencias
- **Eliminación permanente**: Este script eliminará permanentemente todas las carpetas `node_modules` encontradas. Asegúrate de que no necesitas ninguna antes de proceder.
- **Consejo de rendimiento**: Analizar directorios grandes como `C:\` puede llevar mucho tiempo. Usa una ruta más corta para acelerar el proceso.