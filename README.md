## ¿Qué hace?
Un script de Python que organiza automáticamente archivos
en carpetas según el tipo de archivo (PDF, PNG, etc.) y 
la antigüedad — archivos mayores a 30 días van directo a 
una carpeta llamada "Archivo", sin importar el tipo.

## El problema
Antes: como estudiante universitaria acumulé más de 30 
archivos en una sola carpeta — PDFs, tareas, apuntes — 
sin saber cuáles eran recientes ni de qué eran.

Después: cada archivo va a su carpeta según tipo, y los 
olvidados tienen su propio lugar.

## Posibles mejoras
- [ ] Agregar interfaz visual para el usuario
- [ ] Programar ejecución automática cada X días

## ¿Cómo usarlo?
1. Crea una carpeta de prueba con archivos mezclados adentro
2. Cambia la variable `carpeta` en el script por la ruta 
   de tu carpeta
3. Ejecuta: `python organizador.py`
4. Revisa el archivo `log.csv` para ver qué se movió

## Qué aprendí
- **Scope:** Las variables solo existen dentro del bloque donde se crean — moverlas fuera rompía el código.
- **Módulos:** usé `os`, `shutil`, `csv` y `datetime` 
  para leer archivos y determinar rutas con OS, mover archivos con shutil, crear un log con csv y crear una condición de tiempo con datetime
- **Logging:** Un registro en CSV que guarda qué archivo se movió, adónde, y cuándo — sin tener que abrir las carpetas para verificarlo.

## Tecnologías
Python 3 — `os` `shutil` `csv` `datetime`
