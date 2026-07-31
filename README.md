# Ejercicio_Modulo2_Ciberseguridad
**Alumno:** Rodrigo Exequiel Mendoza
**Módulo 2:** Protegiendo el sistema operativo (Windows/Linux)

## 1. Configuración del Aislamiento de Red

![Captura de Red Interna en VirtualBox](/evidencias/configuracion_red.png)

### Justificación Técnica
Para este laboratorio inicial, se ha configurado el adaptador en modo **Red Interna**. La Red Interna funciona como un búnker total. En este modo, la VM no tiene acceso a Internet ni a tu computadora Host. Solo puede hablar con otras máquinas virtuales que estén configuradas en la misma Red Interna. Es el entorno más seguro para análisis de malware o pruebas controladas. 
Se ha descartado por completo el uso del modo **Adaptador Puente**. Este modo hace que la VM se conecte directamente al router de tu casa, como si fuera un dispositivo físico más. Si se utiliza este modo, tu máquina virtual ahora es visible para todos en tu red WiFi, lo que permite que un atacante en internet la encuentre fácilmente si hay una mala configuración. Por normativa de seguridad, se evita este modo en tus primeros laboratorios de seguridad.

## 2. Protección del Estado Inicial (Snapshot)

![Captura del primer Snapshot](/evidencias/snapshot_limpio.png)

**Nombre del Snapshot:** Instalación Base Limpia
**Propósito:** Garantizar un punto de retorno seguro tras la instalación limpia del sistema operativo invitado, permitiendo revertir cualquier configuración errónea o infección por malware durante futuras prácticas.
