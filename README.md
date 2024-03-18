# Incus

Incus is a modern, secure and powerful system container and virtual machine manager.

It provides a unified experience for running and managing full Linux systems inside containers or virtual machines. Incus supports images for a large number of Linux distributions (official Ubuntu images and images provided by the community) and is built around a very powerful, yet pretty simple, REST API. Incus scales from one instance on a single machine to a cluster in a full data center rack, making it suitable for running workloads both for development and in production.

Incus allows you to easily set up a system that feels like a small private cloud. You can run any type of workload in an efficient way while keeping your resources optimized.

Check more info: https://github.com/lxc/incus

# Incus custom images

The aim of this project is to create custom images to help developers to configure development environments quickly.

# Get started

The first step is to install incus into your computer. Incus is available on most common Linux distributions, you can check the documentation to how to install Incus: https://linuxcontainers.org/incus/docs/main/installing/
Once Incus is installed, review the official documentation to set up a development environment in a few steps.

## Debian+PHP+MySQL8 for web development

This image is based in Debian 12 with Apache2 server. It can be configured with any version of PHP, from v5.6 until v8.2. As a database engine it includes MySQL 8.0. It also comes pre-installed with 2 versions of phpMyAdmin compatible with different versions of PHP.

### Main features

- Debian 12 cloud based image.
- Apache2 server.
- This image includes PHP 8.1 by default, but supports all PHP versions since 5.6.
- PHP 8.1 extensions: libapache2-mod-php8.1 php8.1 php8.1-zip php8.1-bz2 php8.1-mysql php8.1-mbstring.
- MySQL Server 8.0 with legacy auth method.
- phpMyAdmin v4.9.11 (PHP 5.5 to 7.4 + MySQL/MariaDB 5.5 and newer)  and phpMyAdmin 5.2.1 (PHP 7.2 and newer + MySQL/MariaDB 5.5 and newer)

### Additional system packages

- nano
- wget
- curl
- openssh-server
- net-tools
- unzip
- rsync
- git 

**IMPORTANT:**

This image is for development purposes not for a production environment. A few things need to be changed to improve security in a production environment.

# Documentation

Official documentation is still in progress. As soon as I can, I'll post the link.