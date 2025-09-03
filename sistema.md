# 🖥️ Sistema

Programas para monitoreo, administración y gestión del sistema Linux.

---

## Monitoreo de procesos

### `btop`
Monitor de procesos en tiempo real con una interfaz visual atractiva.

![btop](https://raw.githubusercontent.com/aristocratos/btop/refs/heads/main/Img/normal.png)

```bash
btop --help

Usage: btop [OPTIONS]

Options:
  -c, --config <file>     Path to a config file
  -d, --debug             Start in debug mode with additional logs and metrics
  -f, --filter <filter>   Set an initial process filter
      --force-utf         Override automatic UTF locale detection
  -l, --low-color         Disable true color, 256 colors only
  -p, --preset <id>       Start with a preset (0-9)
  -t, --tty               Force tty mode with ANSI graph symbols and 16 colors only
      --no-tty            Force disable tty mode
  -u, --update <ms>       Set an initial update rate in milliseconds
  -h, --help              Show this help message and exit
  -V, --version           Show a version message and exit (more with --version)
```
Repo: [https://github.com/aristocratos/btop](https://github.com/aristocratos/btop)


### `htop`
Monitor interactivo de procesos y recursos del sistema.
```bash
htop
```

### `top`
Monitor básico de procesos en tiempo real.
```bash
top
```

### `ps`
Muestra información sobre los procesos en ejecución.
```bash
ps aux
```

### `pstree`
Muestra los procesos en forma de árbol jerárquico.
```bash
pstree
```

---

## Información del sistema

### `neofetch`
Muestra información del sistema de forma visualmente atractiva.
```bash
neofetch
```

### `uname`
Información básica del kernel y sistema.
```bash
uname -a
```

### `lscpu`
Información detallada del procesador.
```bash
lscpu
```

### `lsblk`
Lista los dispositivos de bloque (discos, particiones).
```bash
lsblk
```

### `df`
Muestra el espacio usado y disponible en los sistemas de archivos.
```bash
df -h
```

### `free`
Información sobre la memoria RAM y swap.
```bash
free -h
```

---

## Gestión de servicios

### `systemctl`
Control de servicios del sistema con systemd.
```bash
systemctl status nginx
```

### `journalctl`
Visualización de logs del sistema.
```bash
journalctl -u ssh
```

---

## Procesos y tareas

### `kill`
Termina procesos por PID.
```bash
kill 1234
```

### `killall`
Termina procesos por nombre.
```bash
killall firefox
```

### `jobs`
Muestra trabajos en segundo plano.
```bash
jobs
```

### `nohup`
Ejecuta comandos que persisten después de cerrar la terminal.
```bash
nohup python script.py &
```

---

## Usuarios y permisos

### `who`
Muestra quién está conectado al sistema.
```bash
who
```

### `id`
Información sobre el usuario actual y sus grupos.
```bash
id
```

### `sudo`
Ejecuta comandos con privilegios de administrador.
```bash
sudo apt update
```

### `su`
Cambia al usuario root o a otro usuario.
```bash
su -
```

---

## Variables de entorno

### `env`
Muestra todas las variables de entorno.
```bash
env
```

### `export`
Define variables de entorno.
```bash
export PATH=$PATH:/nueva/ruta
```

---

[← Volver al inicio](README.md)