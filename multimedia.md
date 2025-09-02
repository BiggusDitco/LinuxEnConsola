# 🎵 Multimedia

Herramientas para trabajar con audio, video, imágenes y contenido multimedia desde la consola.

---

## Reproductores de audio

* **`mpv`**
    * Reproductor multimedia minimalista y potente.
    * **Ejemplo:** Reproduce un archivo de video y un playlist, ajustando el volumen y añadiendo subtítulos.
        ```bash
        mpv --volume=80 --sub-file=subtitulos.srt video.mp4 cancion.mp3
        ```
    * **Repo:** [https://github.com/mpv-player/mpv](https://github.com/mpv-player/mpv)

* **`moc` (Music on Console)**
    * Reproductor de audio con interfaz de consola estilo ncurses.
    * **Ejemplo:** Inicia el reproductor y añade todos los archivos MP3 de un directorio a la lista de reproducción.
        ```bash
        mocp -S ~/Musica/
        ```
    * **Repo:** [https://github.com/jonas-k/moc](https://github.com/jonas-k/moc)

* **`cmus`**
    * Reproductor de música ligero y rápido.
    * **Ejemplo:** Inicia cmus y reproduce la primera canción del directorio.
        ```bash
        cmus ~/Musica/
        ```
    * **Repo:** [https://github.com/cmus/cmus](https://github.com/cmus/cmus)

* **`mpg123`**
    * Reproductor específico para archivos MP3.
    * **Ejemplo:** Reproduce un archivo MP3 de una URL.
        ```bash
        mpg123 [https://ejemplo.com/cancion.mp3](https://ejemplo.com/cancion.mp3)
        ```
    * **Repo:** [https://github.com/mpg123/mpg123](https://github.com/mpg123/mpg123)

---

## Conversión y edición de audio

* **`ffmpeg`**
    * Herramienta completa para conversión y edición multimedia.
    * **Ejemplo:** Convierte un video de MP4 a MKV con un códec de video diferente y mantiene el audio original.
        ```bash
        ffmpeg -i input.mp4 -c:v libx264 -c:a copy output.mkv
        ```
    * **Repo:** [https://github.com/FFmpeg/FFmpeg](https://github.com/FFmpeg/FFmpeg)

* **`sox`**
    * "Navaja suiza" para procesamiento de audio.
    * **Ejemplo:** Recorta un archivo de audio a 10 segundos y le aplica un efecto de reverberación.
        ```bash
        sox input.wav output.wav trim 0 10 reverb 50 50
        ```
    * **Repo:** [https://github.com/sox-audio/sox](https://github.com/sox-audio/sox)

* **`lame`**
    * Codificador de MP3 de alta calidad.
    * **Ejemplo:** Codifica un archivo WAV a MP3 con calidad VBR (bitrate variable) alta.
        ```bash
        lame -V 0 input.wav output.mp3
        ```
    * **Repo:** [https://github.com/Boardwalker/LAME](https://github.com/Boardwalker/LAME)

* **`flac`**
    * Codificador/decodificador de audio sin pérdida.
    * **Ejemplo:** Decodifica un archivo FLAC a WAV.
        ```bash
        flac -d input.flac -o output.wav
        ```
    * **Repo:** [https://github.com/xiph/flac](https://github.com/xiph/flac)

---

## Información de archivos multimedia

* **`mediainfo`**
    * Información detallada sobre archivos multimedia.
    * **Ejemplo:** Muestra información técnica detallada de un archivo de video.
        ```bash
        mediainfo video.mp4
        ```
    * **Repo:** [https://github.com/MediaArea/MediaInfo](https://github.com/MediaArea/MediaInfo)

* **`exiftool`**
    * Lee y modifica metadatos de archivos multimedia.
    * **Ejemplo:** Muestra los metadatos de una foto y extrae la fecha de creación.
        ```bash
        exiftool foto.jpg
        exiftool -CreateDate foto.jpg
        ```
    * **Repo:** [https://github.com/exiftool/exiftool](https://github.com/exiftool/exiftool)

* **`file`**
    * Identifica el tipo de archivo.
    * **Ejemplo:** Identifica el tipo de un archivo.
        ```bash
        file archivo.mp4
        ```
    * **Repo:** No es un proyecto de GitHub, es parte de la mayoría de los sistemas operativos Linux.

---

## Captura de pantalla

* **`scrot`**
    * Captura de pantalla simple.
    * **Ejemplo:** Captura una pantalla con un retraso de 5 segundos.
        ```bash
        scrot -d 5 screenshot.png
        ```
    * **Repo:** [https://github.com/Resurrect-Project/scrot](https://github.com/Resurrect-Project/scrot)

* **`import`**
    * Captura de pantalla (parte de ImageMagick).
    * **Ejemplo:** Captura una ventana específica haciendo clic en ella después de ejecutar el comando.
        ```bash
        import screenshot.png
        ```
    * **Repo:** [https://github.com/ImageMagick/ImageMagick](https://github.com/ImageMagick/ImageMagick)

---

## Streaming y descarga

* **`youtube-dl` / `yt-dlp`**
    * Descarga videos de YouTube y otras plataformas.
    * **Ejemplo:** Descarga un video de YouTube en la mejor calidad disponible y como archivo de audio.
        ```bash
        yt-dlp -f bestvideo+bestaudio --merge-output-format mp4 [https://youtube.com/watch?v=VIDEO_ID](https://youtube.com/watch?v=VIDEO_ID)
        yt-dlp -x --audio-format mp3 [https://youtube.com/watch?v=VIDEO_ID](https://youtube.com/watch?v=VIDEO_ID)
        ```
    * **Repo:** [https://github.com/yt-dlp/yt-dlp](https://github.com/yt-dlp/yt-dlp)

* **`streamlink`**
    * Reproduce streams en vivo desde la consola.
    * **Ejemplo:** Reproduce un stream de Twitch en la mejor calidad en mpv.
        ```bash
        streamlink [https://twitch.tv/canal](https://twitch.tv/canal) best
        ```
    * **Repo:** [https://github.com/streamlink/streamlink](https://github.com/streamlink/streamlink)

---

## Análisis de audio

* **`audacity`**
    * Edición de audio en lotes.
    * **Ejemplo:** Procesa varios archivos de audio aplicando un script de Audacity.
        ```bash
        audacity --batch-process --script-args "inputfiles=*.wav" script.ny
        ```
    * **Repo:** [https://github.com/audacity/audacity](https://github.com/audacity/audacity)

* **`spectacle`** (Este es un error, el comando correcto es con `sox` como en el ejemplo original).
    * Análisis espectral de audio.
    * **Ejemplo:** Genera un espectrograma de un archivo de audio WAV.
        ```bash
        sox archivo.wav -n spectrogram
        ```
    * **Repo:** [https://github.com/sox-audio/sox](https://github.com/sox-audio/sox)

---

## Códecs y formatos

* **`x264`**
    * Codificador de video H.264.
    * **Ejemplo:** Codifica un archivo YUV a H.264 con un factor de calidad constante (CRF) de 20.
        ```bash
        x264 --crf 20 input.yuv -o output.mp4
        ```
    * **Repo:** [https://github.com/mirror/x264](https://github.com/mirror/x264)

* **`x265`**
    * Codificador de video H.265/HEVC.
    * **Ejemplo:** Codifica un archivo YUV a H.265/HEVC.
        ```bash
        x265 input.yuv output.hevc
        ```
    * **Repo:** [https://github.com/videolan/x265](https://github.com/videolan/x265)

---

## Subtítulos

* **`subliminal`**
    * Descarga automática de subtítulos.
    * **Ejemplo:** Descarga subtítulos en español para una película.
        ```bash
        subliminal download -l es movie.mp4
        ```
    * **Repo:** [https://github.com/subliminal-tools/subliminal](https://github.com/subliminal-tools/subliminal)

* **`ccextractor`**
    * Extrae subtítulos cerrados de videos.
    * **Ejemplo:** Extrae subtítulos de un archivo de video MPEG-TS.
        ```bash
        ccextractor video.ts
        ```
    * **Repo:** [https://github.com/CCExtractor/ccextractor](https://github.com/CCExtractor/ccextractor)

---

## Audio en vivo

* **`arecord`**
    * Grabación de audio desde micrófono.
    * **Ejemplo:** Graba 10 segundos de audio del micrófono con una frecuencia de muestreo de 44.1 kHz.
        ```bash
        arecord -d 10 -f S16_LE -r 44100 grabacion.wav
        ```
    * **Repo:** No es un proyecto de GitHub, es parte de `alsa-utils`. Puedes encontrar su código en el repositorio de ALSA: [https://github.com/alsa-project/alsa-utils](https://github.com/alsa-project/alsa-utils)