# 🛠️ Utilidades

Herramientas esenciales para búsqueda, compresión, manejo de archivos y tareas cotidianas.

---

## Navegación y archivos

### `ls`
Lista archivos y directorios.
```bash
ls -la
```

### `cd`
Cambia de directorio.
```bash
cd /home/usuario
```

### `pwd`
Muestra la ruta del directorio actual.
```bash
pwd
```

### `tree`
Muestra la estructura de directorios en forma de árbol.
```bash
tree
```

### `find`
Busca archivos y directorios.
```bash
find /home -name "*.txt"
```

### `locate`
Búsqueda rápida de archivos por nombre.
```bash
locate archivo.txt
```

---

## Visualización de archivos

### `cat`
Muestra el contenido completo de un archivo.
```bash
cat archivo.txt
```

### `less`
Visualiza archivos grandes de forma paginada.
```bash
less archivo.txt
```

### `head`
Muestra las primeras líneas de un archivo.
```bash
head -10 archivo.txt
```

### `tail`
Muestra las últimas líneas de un archivo.
```bash
tail -f /var/log/syslog
```

### `bat`
Visualizador de archivos con resaltado de sintaxis.
```bash
bat archivo.py
```

---

## Búsqueda en archivos

### `grep`
Busca texto dentro de archivos.
```bash
grep "error" /var/log/syslog
```

### `rg` (ripgrep)
Búsqueda de texto ultrarrápida.
```bash
rg "función" src/
```

### `ack`
Herramienta de búsqueda optimizada para programadores.
```bash
ack "class" --python
```

---

## Manipulación de archivos

### `cp`
Copia archivos y directorios.
```bash
cp archivo.txt /destino/
```

### `mv`
Mueve o renombra archivos.
```bash
mv archivo.txt nuevo_nombre.txt
```

### `rm`
Elimina archivos y directorios.
```bash
rm -rf directorio/
```

### `mkdir`
Crea directorios.
```bash
mkdir -p ruta/completa/nueva
```

### `touch`
Crea archivos vacíos o actualiza timestamps.
```bash
touch nuevo_archivo.txt
```

### `ln`
Crea enlaces simbólicos.
```bash
ln -s /ruta/original /ruta/enlace
```

---

## Compresión y archivos

### `tar`
Empaqueta y comprime archivos.
```bash
tar -czf archivo.tar.gz directorio/
```

### `zip`
Crea archivos ZIP.
```bash
zip -r archivo.zip directorio/
```

### `unzip`
Extrae archivos ZIP.
```bash
unzip archivo.zip
```

### `gzip`
Comprime archivos individuales.
```bash
gzip archivo.txt
```

---

## Análisis de espacio

### `du`
Analiza el uso de espacio en disco.
```bash
du -sh *
```

### `ncdu`
Analizador interactivo de uso de disco.
```bash
ncdu
```

---

## Comparación y diferencias

### `diff`
Compara archivos línea por línea.
```bash
diff archivo1.txt archivo2.txt
```

### `vimdiff`
Comparador visual de archivos.
```bash
vimdiff archivo1.txt archivo2.txt
```

---

## Procesamiento de texto

### `sort`
Ordena líneas de texto.
```bash
sort archivo.txt
```

### `uniq`
Elimina líneas duplicadas.
```bash
sort archivo.txt | uniq
```

### `wc`
Cuenta líneas, palabras y caracteres.
```bash
wc -l archivo.txt
```

### `cut`
Extrae columnas de texto.
```bash
cut -d',' -f1 datos.csv
```

### `awk`
Procesamiento avanzado de texto.
```bash
awk '{print $1}' archivo.txt
```

### `sed`
Editor de flujo para filtrar y transformar texto.
```bash
sed 's/viejo/nuevo/g' archivo.txt
```

---

## Fechas y tiempo

### `date`
Muestra o establece la fecha del sistema.
```bash
date "+%Y-%m-%d %H:%M:%S"
```

### `cal`
Muestra un calendario.
```bash
cal
```

---

[← Volver al inicio](README.md)