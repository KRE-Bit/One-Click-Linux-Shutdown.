# One-Click-Linux-Shutdown.
You can shot down your linux computer where ever you are, from america to china. Try it 


# ⚡ One-Click Linux Server Shutdown (vía SSH)

Un script en Batch ligero y seguro para apagar servidores Linux de forma remota desde Windows con un solo clic, sin necesidad de usar programas de Escritorio Remoto.

Ideal para servidores NAS caseros (como Linux Mint o Ubuntu) gestionados a través de redes privadas virtuales como Tailscale. Ayuda a prevenir la corrupción de discos duros mecánicos garantizando un apagado seguro antes de cortar la energía.

## 🚀 Requisitos Previos
Para que este script funcione sin detenerse a pedir contraseñas, necesitas configurar tu servidor Linux:
1. Tener `openssh-server` instalado.
2. Haber generado llaves SSH (`ssh-keygen`) entre tu Windows y tu servidor Linux.
3. Configurar una excepción en el servidor con: 
   `echo "$USER ALL=(ALL) NOPASSWD: /sbin/shutdown" | sudo tee /etc/sudoers.d/apagado_automatico`

## 🛠️ Uso
1. Descarga el archivo `Apagar_Servidor.bat`.
2. Haz clic derecho y selecciona "Editar".
3. Cambia `TU_USUARIO` por tu usuario de Linux y `TU_IP` por la IP de tu servidor (Local o Tailscale).
4. ¡Haz doble clic y listo!
