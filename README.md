# 🐘 XAMPP Docker Stack + Firma Electrónica SV

Este proyecto es un stack completo de desarrollo PHP al estilo **XAMPP**, containerizado con **Docker**, que incluye soporte para **firma electrónica según normativa de El Salvador**, ideal para entornos de desarrollo y pruebas con **facturación electrónica (SVFE)**.

## 🚀 Servicios incluidos

| Servicio       | Imagen                           | Puerto | Descripción |
|----------------|----------------------------------|--------|-------------|
| Apache + PHP   | `chrasc/xampp-docker-apache-php` | 8080   | Servidor web con PHP 8.x |
| MariaDB        | `mariadb:latest`                 | 3306   | Base de datos |
| phpMyAdmin     | `phpmyadmin/phpmyadmin`          | 8081   | Interfaz web para MariaDB |
| Firmador SVFE  | `chrasc/svfe-api-firmador`       | 8113   | Microservicio de firma electrónica |

---

## 📁 Estructura del proyecto

```plaintext
mi-stack-docker/
├── docker-compose.yml         ← Configuración del stack
├── htdocs/                    ← Tu código PHP va aquí
├── apache/default.conf        ← Configuración de Apache
├── temp/                      ← Carpeta para subir certificados (.crt/.key)
├── .gitignore                 ← Archivos ignorados en Git
└── README.md                  ← Este archivo
