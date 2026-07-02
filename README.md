# Proyecto DOMUX - DevOps

Este repositorio contiene la arquitectura de software para **DOMUX**, un sistema SaaS multi-tenant para operación residencial, desarrollado como parte del programa de Análisis y Desarrollo de Software (ADSO) en el SENA.

## Descripción del Proyecto
DOMUX centraliza los accesos peatonales, vehiculares, gestión de visitantes, PQRS y auditoría en tiempo real, diseñado para modernizar la administración de conjuntos residenciales en Colombia.

## Arquitectura Técnica
El proyecto implementa un entorno containerizado para garantizar consistencia entre desarrollo y producción:

* **Frontend**: Interfaz de usuario servida mediante **Nginx** (Alpine).
* **Backend**: Lógica de servidor desarrollada en **Python** (Flask).
* **Gestión de Contenedores**: Orquestación mediante **Docker** y **Docker Compose**.

## Cómo ejecutar el proyecto
Para levantar los servicios en tu entorno local y para ejecuta el proyecto:

```bash
# Construir y levantar los contenedores
sudo docker-compose up -d --build
Una vez iniciados, la aplicación estará disponible en http://localhost:8080.
