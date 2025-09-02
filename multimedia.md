# 🎵 Multimedia

Herramientas para trabajar con audio, video, imágenes y contenido multimedia desde la consola.

---

## Reproductores de audio

### `mpv`
Reproductor multimedia minimalista y potente.
```bash
mpv cancion.mp3
```

### `moc` (Music on Console)
Reproductor de audio con interfaz de consola estilo ncurses.
```bash
mocp
```

### `cmus`
Reproductor de música ligero y rápido.
```bash
cmus
```

### `mpg123`
Reproductor específico para archivos MP3.
```bash
mpg123 archivo.mp3
```

---

## Conversión y edición de audio

### `ffmpeg`
Herramienta completa para conversión y edición multimedia.
```bash
ffmpeg -i input.mp4 -c:v libx264 output.mp4
```

### `sox`
"Navaja suiza" para procesamiento de audio.
```bash
sox input.wav output.mp3
```

### `lame`
Codificador de MP3 de alta calidad.
```bash
lame -V 0 input.wav output.mp3
```

### `flac`
Codificador/decodificador de audio sin pérdida.
```bash
flac input.wav
```

---

## Información de archivos multimedia

### `mediainfo`
Información detallada sobre archivos multimedia.
```bash
mediainfo video.mp4
```

### `exiftool`
Lee y modifica metadatos de archivos multimedia.
```bash
exiftool foto.jpg
```

### `file`
Identifica el tipo de archivo.
```bash
file archivo.mp3
```

---

## Reproductores de video

### `mpv`
Reproductor de video desde consola.
```bash
mpv video.mp4
```

### `vlc`
VLC en modo consola (cvlc).
```bash
cvlc --intf dummy video.mp4
```

### `mplayer`
Reproductor clásico de video.
```bash
mplayer video.avi
```

---

## Procesamiento de imágenes

### `imagemagick` (convert)
Edición y conversión de imágenes.
```bash
convert imagen.jpg -resize 800x600 imagen_pequena.jpg
```

### `mogrify`
Modificación en lote de imágenes.
```bash
mogrify -resize 50% *.jpg
```

### `identify`
Información sobre archivos de imagen.
```bash
identify imagen.jpg
```

### `feh`
Visualizador ligero de imágenes.
```bash
feh imagen.jpg
```

---

## Captura de pantalla

### `scrot`
Captura de pantalla simple.
```bash
scrot screenshot.png
```

### `import`
Captura de pantalla (parte de ImageMagick).
```bash
import screenshot.png
```

---

## Streaming y descarga

### `youtube-dl` / `yt-dlp`
Descarga videos de YouTube y otras plataformas.
```bash
yt-dlp https://youtube.com/watch?v=VIDEO_ID
```

### `streamlink`
Reproduce streams en vivo desde la consola.
```bash
streamlink https://twitch.tv/canal best
```

---

## Análisis de audio

### `audacity` (modo batch)
Edición de audio en lotes.
```bash
audacity --batch-process
```

### `spectacle`
Análisis espectral de audio.
```bash
sox archivo.wav -n spectrogram
```

---

## Códecs y formatos

### `x264`
Codificador de video H.264.
```bash
x264 --crf 20 input.yuv -o output.mp4
```

### `x265`
Codificador de video H.265/HEVC.
```bash
x265 input.yuv output.hevc
```

---

## Subtítulos

### `subliminal`
Descarga automática de subtítulos.
```bash
subliminal download -l es movie.mp4
```

### `ccextractor`
Extrae subtítulos cerrados de videos.
```bash
ccextractor video.ts
```

---

## Audio en vivo

### `arecord`
Grabación de audio desde micrófono.
```bash
arecord -f cd audio.wav
```

### `aplay`
Reproducción de archivos de audio.
```bash
aplay archivo.wav
```

### `alsamixer`
Control de volumen y mezclador de ALSA.
```bash
alsamixer
```

---

## Visualización de audio

### `cava`
Visualizador de espectro de audio.
```bash
cava
```

### `vis`
Visualizador de música basado en ncurses.
```bash
vis
```

---

[← Volver al inicio](README.md)