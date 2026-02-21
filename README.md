# Streamingserver
Descripcion de servidor casero para hogar compartido de forma segura usando Tailscale/WireGuard

Este proyecto explica cómo montar un servidor multimedia en casa usando Jellyfin y compartirlo de forma segura con amigos y familiares a través de Tailscale, sin necesidad de abrir puertos en el router.

Concepros Básicos

Jellyfin → Servidor multimedia open-source tipo Netflix personal.

Tailscale → VPN tipo mesh basada en WireGuard que permite acceso remoto seguro sin configurar NAT o port forwarding.


PC con Windows 10 LTSC Enterprise

8GB RAM recomendados

Espacio suficiente para biblioteca multimedia

Conexión estable a internet

Cuenta gratuita en Tailscale

ESTRUCTURA DE CARPETAS
D:\Media
 ├── Peliculas
 │    └── Interstellar (2014)
 │         └── Interstellar (2014).mkv
 │
 └── Series
      └── Breaking Bad
           └── Season 01
                └── Breaking Bad - S01E01.mkv



                Acceso remoto

Tus amigos/familia deben:

Instalar Tailscale

Iniciar sesión (o aceptar invitación a tu red)

Acceder a:

http://IP_TAILSCALE:8096


SEGURIDAD:


Configuración de Seguridad en Windows
Firewall

Verificar que Windows permita Jellyfin:

Panel de Control

Firewall de Windows

Permitir aplicación

Confirmar que Jellyfin esté habilitado en red privada

NO abrir puertos en el router.



Aceleración por hardware en Windows

Si tu PC tiene:

Intel Quick Sync

GPU NVIDIA (NVENC)

GPU AMD

En Jellyfin:

Dashboard → Playback → Transcoding

Activar:

Hardware Acceleration (Opcional)



Dispositivos compatibles

Clientes Jellyfin disponibles para:

Android

iOS

Smart TV

Fire TV

Navegador web

Solo deben estar conectados a Tailscale.





En Windows funciona muy bien con Quick Sync y NVENC.
<img width="1292" height="658" alt="image" src="https://github.com/user-attachments/assets/acdf960e-e3ff-4f9c-9f70-95560a0d9de2" />

