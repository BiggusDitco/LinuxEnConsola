# 🌐 Red

Herramientas para conectividad, descargas, pruebas de red y comunicación.

---

## Conectividad y pruebas

### `ping`
Prueba la conectividad con un host.
```bash
ping google.com
```

### `curl`
Transfiere datos desde o hacia un servidor.
```bash
curl https://api.ejemplo.com/datos
```

### `wget`
Descarga archivos desde la web.
```bash
wget https://ejemplo.com/archivo.zip
```

### `traceroute`
Muestra la ruta que siguen los paquetes hasta un destino.
```bash
traceroute google.com
```

### `mtr`
Combinación de ping y traceroute en tiempo real.
```bash
mtr google.com
```

### `nmap`
Escáner de puertos y redes.
```bash
nmap -sP 192.168.1.0/24
```

---

## Información de red

### `ip`
Configuración y información de interfaces de red.
```bash
ip addr show
```

### `ifconfig`
Configuración clásica de interfaces de red.
```bash
ifconfig
```

### `netstat`
Muestra conexiones de red, puertos abiertos y estadísticas.
```bash
netstat -tuln
```

### `ss`
Versión moderna de netstat para mostrar sockets.
```bash
ss -tuln
```

### `lsof`
Lista archivos abiertos, incluyendo conexiones de red.
```bash
lsof -i :80
```

---

## Transferencia de archivos

### `scp`
Copia archivos de forma segura entre hosts.
```bash
scp archivo.txt usuario@servidor:/ruta/destino/
```

### `rsync`
Sincronización eficiente de archivos.
```bash
rsync -avz carpeta/ usuario@servidor:/backup/
```

### `sftp`
Transferencia segura de archivos vía SSH.
```bash
sftp usuario@servidor
```

---

## Conexiones remotas

### `ssh`
Conexión segura a servidores remotos.
```bash
ssh usuario@servidor
```

### `ssh-keygen`
Genera claves SSH para autenticación.
```bash
ssh-keygen -t rsa -b 4096
```

### `ssh-copy-id`
Copia la clave pública SSH a un servidor.
```bash
ssh-copy-id usuario@servidor
```

---

## Análisis de tráfico

### `tcpdump`
Captura y analiza paquetes de red.
```bash
sudo tcpdump -i eth0 port 80
```

### `wireshark` / `tshark`
Analizador de protocolos de red (versión consola).
```bash
tshark -i eth0 -f "port 443"
```

### `iftop`
Monitor de ancho de banda en tiempo real.
```bash
sudo iftop
```

### `nethogs`
Muestra el uso de ancho de banda por proceso.
```bash
sudo nethogs
```

---

## DNS y resolución

### `dig`
Consultas DNS avanzadas.
```bash
dig google.com MX
```

### `nslookup`
Consultas DNS básicas.
```bash
nslookup google.com
```

### `host`
Búsqueda simple de DNS.
```bash
host google.com
```

---

## Servicios web

### `httpie`
Cliente HTTP amigable para APIs.
```bash
http GET https://api.ejemplo.com/users
```

### `lynx`
Navegador web de texto.
```bash
lynx https://ejemplo.com
```

### `w3m`
Navegador web de texto con soporte para imágenes.
```bash
w3m https://ejemplo.com
```

---

## Correo electrónico

### `mail`
Envío y recepción de correo desde consola.
```bash
echo "Mensaje" | mail -s "Asunto" usuario@ejemplo.com
```

### `mutt`
Cliente de correo completo para consola.
```bash
mutt
```

---

## Firewall y seguridad

### `ufw`
Firewall simplificado para Ubuntu.
```bash
sudo ufw enable
```

### `iptables`
Configuración avanzada del firewall.
```bash
sudo iptables -L
```

---

## Redes inalámbricas

### `iwconfig`
Configuración de interfaces Wi-Fi.
```bash
iwconfig
```

### `nmcli`
Control de NetworkManager desde consola.
```bash
nmcli device wifi list
```

---

[← Volver al inicio](README.md)