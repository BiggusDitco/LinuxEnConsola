# 🔒 Seguridad

Herramientas para cifrado, análisis de seguridad, gestión de contraseñas y protección del sistema.

---

## Cifrado y criptografía

### `gpg`
Cifrado y firma digital con GNU Privacy Guard.
```bash
gpg --encrypt --recipient usuario@ejemplo.com archivo.txt
```

### `openssl`
Herramientas criptográficas y certificados SSL.
```bash
openssl rand -base64 32
```

### `age`
Herramienta moderna de cifrado de archivos.
```bash
age -r public_key.txt archivo.txt > archivo.age
```

---

## Hashes y verificación

### `sha256sum`
Calcula checksums SHA-256.
```bash
sha256sum archivo.iso
```

### `md5sum`
Calcula checksums MD5.
```bash
md5sum archivo.tar.gz
```

### `hashcat`
Herramienta avanzada de cracking de hashes.
```bash
hashcat -m 0 hashes.txt wordlist.txt
```

---

## Gestión de contraseñas

### `pass`
Gestor de contraseñas estándar de Unix.
```bash
pass insert Email/gmail.com
```

### `pwgen`
Generador de contraseñas seguras.
```bash
pwgen -s 16 1
```

### `keepassxc-cli`
Cliente de consola para KeePassXC.
```bash
keepassxc-cli show database.kdbx Entry
```

---

## Análisis de vulnerabilidades

### `nmap`
Escáner de puertos y vulnerabilidades.
```bash
nmap -sV -sC target.com
```

### `nikto`
Escáner de vulnerabilidades web.
```bash
nikto -h https://ejemplo.com
```

### `lynis`
Auditor de seguridad del sistema.
```bash
sudo lynis audit system
```

---

## Monitoreo y logs

### `fail2ban-client`
Control del sistema de protección fail2ban.
```bash
sudo fail2ban-client status
```

### `logwatch`
Análisis automático de logs del sistema.
```bash
sudo logwatch --detail high
```

### `aide`
Sistema de detección de intrusiones basado en archivos.
```bash
sudo aide --check
```

---

## Red y firewall

### `ufw`
Firewall simplificado.
```bash
sudo ufw status verbose
```

### `iptables`
Configuración avanzada del firewall.
```bash
sudo iptables -L -n -v
```

### `wireshark` / `tshark`
Análisis de tráfico de red.
```bash
sudo tshark -i eth0 -f "port 443"
```

---

## Autenticación

### `ssh-keygen`
Generación de claves SSH.
```bash
ssh-keygen -t ed25519 -C "email@ejemplo.com"
```

### `ssh-agent`
Agente de autenticación SSH.
```bash
ssh-add ~/.ssh/id_rsa
```

### `google-authenticator`
Configuración de autenticación de dos factores.
```bash
google-authenticator
```

---

## Análisis forense

### `strings`
Extrae cadenas de texto de archivos binarios.
```bash
strings binario | grep -i password
```

### `hexdump`
Muestra contenido de archivos en hexadecimal.
```bash
hexdump -C archivo.bin
```

### `volatility`
Análisis de memoria RAM.
```bash
volatility -f memory.dump imageinfo
```

---

## Limpieza y privacidad

### `shred`
Eliminación segura de archivos.
```bash
shred -vfz -n 3 archivo_secreto.txt
```

### `wipe`
Limpieza segura de espacios libres.
```bash
wipe -rf directorio_sensible/
```

### `bleachbit`
Limpieza de archivos temporales y privacidad.
```bash
bleachbit --clean system.tmp
```

---

## Permisos y acceso

### `chmod`
Modificación de permisos de archivos.
```bash
chmod 600 archivo_privado.txt
```

### `chown`
Cambio de propietario de archivos.
```bash
sudo chown usuario:grupo archivo.txt
```

### `umask`
Configuración de permisos por defecto.
```bash
umask 077
```

---

## Certificados SSL/TLS

### `certbot`
Cliente de Let's Encrypt para certificados SSL.
```bash
sudo certbot certonly --standalone -d ejemplo.com
```

### `openssl`
Verificación de certificados SSL.
```bash
openssl s_client -connect ejemplo.com:443
```

---

## Backup seguro

### `rsync`
Sincronización segura con cifrado.
```bash
rsync -avz -e ssh datos/ usuario@servidor:/backup/
```

### `tar` + `gpg`
Backup cifrado con compresión.
```bash
tar czf - directorio/ | gpg -c > backup.tar.gz.gpg
```

---

## Análisis de malware

### `clamav`
Escáner de antivirus de código abierto.
```bash
clamscan -r /home/usuario/
```

### `rkhunter`
Detector de rootkits.
```bash
sudo rkhunter --check
```

### `chkrootkit`
Verificador de rootkits alternativo.
```bash
sudo chkrootkit
```

---

[← Volver al inicio](README.md)