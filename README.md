# Laboratorio de Sistemas Operativos: Entorno Multi-Servicio Controlado

## 👥 Integrante
* Estudiante: [Juan Esteban Aguirre Castañeda] 
* Codigo: [202459676]
* Plan: [3743]

## 📝 Descripción del Proyecto
Este proyecto consiste en el diseño, despliegue y administración de un entorno multi-servicio controlado basado en contenedores Docker, ejecutado de forma nativa sobre el núcleo de Linux utilizando el Subsistema de Windows para Linux (WSL2) en una distribución Ubuntu.

## 🏗️ Arquitectura del Entorno
El sistema se compone de 5 servicios aislados que coexisten en una red privada virtual de tipo `bridge` gestionada por Docker Compose:
1. **Nginx (Puerto 8080):** Servidor web que actúa como proxy.
2. **Node.js (Puerto 3000):** Servidor de aplicaciones con Express.
3. **PostgreSQL (Puerto 5432 - Interno):** Base de datos relacional con volumen persistente.
4. **pgAdmin 4 (Puerto 5050):** Panel gráfico de administración de la base de datos.
5. **Jupyter Lab (Puerto 8888):** Entorno para ciencia de datos y ejecución de notebooks.

## 📋 Requisitos Previos
* Windows 10/11 con soporte de Virtualización de CPU habilitado en BIOS.
* WSL2 con distribución Ubuntu instalada.
* Docker Desktop configurado con el motor de WSL2.
* Cuenta activa en GitHub.

## 🚀 Pasos de Instalación y Despliegue
1. Clonar este repositorio:
   ```bash
   git clone https://github.com/Jeac2506/mi-proyecto-docker.git
   cd mi-proyecto-docker
