# Incus

Incus es un gestor de máquinas virtuales y contenedores moderno, seguro y potente.

Proporciona una experiencia unificada para ejecutar y administrar sistemas Linux dentro de contenedores o máquinas virtuales. Incus admite imágenes para una gran cantidad de distribuciones Linux (imágenes oficiales de Ubuntu e imágenes proporcionadas por la comunidad).

Incus te permite configurar fácilmente un sistema que parece una pequeña nube privada. Puede ejecutar cualquier tipo de carga de trabajo de manera eficiente mientras mantiene sus recursos optimizados.

Puede consultar más información desde el siguiente link: https://github.com/lxc/incus

# Imágenes de Incus personalizadas

El objetivo de este proyecto es crear imágenes personalizadas que permitan a otros desarrolladores configurar entornos de desarrollo de forma rápida.

# Comenzar

El primer paso es instalar Incus en una máquina. Incus está disponible en la mayoria de distribuciones Linux, puedes consultar la documentación de cómo instalar Incus desde el link: https://linuxcontainers.org/incus/docs/main/installing/
Una vez que Incus esté instalado, puedes comenzar a configurar el entorno de desarrollo. Revisa la documentación oficial para aprender a configurar el entorno en pocos pasos.

## Debian+PHP+MySQL8 para desarrollo web

Esta imagen está basada en Debian 12 con Apache2 server. Puede ser configurada con cualquier versión de PHP, desde la v5.6 hasta la v8.3. Como motor de base de datos incluye MySQL 8.0. Además, viene preconfigurada con 2 versiones de phpMyAdmin compatible con versiones diferentes de PHP.

### Principales características

- Imagen basada en Debian 12 cloud.
- Servidor web Apache2.
- Esta imagen incluye PHP 8.1 por defecto, pero soporta desde la versión de PHP 5.6.
- Extensiones de PHP 8.1: libapache2-mod-php8.1 php8.1 php8.1-zip php8.1-bz2 php8.1-mysql php8.1-mbstring.
- Servidor de base de datos MySQL 8.0 con método de autenticación heredado (legacy auth method).
- phpMyAdmin v4.9.11 (PHP 5.5 to 7.4 + MySQL/MariaDB 5.5 y actual) y phpMyAdmin 5.2.1 (PHP 7.2 y actual + MySQL/MariaDB 5.5 y actual).

### Paquetes del sistema adicionales

- nano
- wget
- curl
- openssh-server
- net-tools
- unzip
- rsync
- git 

**IMPORTANTE:**

Esta imagen es para fines de desarrollo, no para un entorno de producción real. Es necesario modificar algunos parámetros para mejorar la seguridad para entornos de producción.

# Documentación

La documentación oficial la puedes encontrar en: https://rubisof.com/proyectos/imagenes-incus-personalizadas/docs
