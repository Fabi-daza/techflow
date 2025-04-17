# Proyecto CI/CD con Jenkins y JSON Server

Este proyecto fue desarrollado como una prueba de concepto para implementar un flujo de integración continua (CI/CD) utilizando **Jenkins** en una instalación local.

## 🛠 Tecnologías utilizadas

- **Jenkins** (instalado localmente)
- **Node.js** y **npm**
- **json-server** para simular una API REST
- **Git** y **GitHub** como repositorio remoto
- **Jenkinsfile** para definir el pipeline

## 🚀 Flujo del pipeline

El pipeline definido en `Jenkinsfile` realiza los siguientes pasos:

1. **Checkout del código** desde GitHub.
2. **Instalación de dependencias** con `npm install`.
3. **Ejecución de pruebas** automáticas (pendiente de implementación o en proceso de revisión).

## 📄 Evidencia

Se adjunta un documento `evidencia.pdf` con **pantallazos del proceso de ejecución del pipeline**, validando cada una de las etapas configuradas.

## 🔧 Requisitos para ejecución local

1. Tener instalado:
   - Node.js (v18 o superior)
   - npm
   - Jenkins
   - Git

2. Clonar el repositorio:
   ```bash
   git clone https://github.com/Fabi-daza/techflow.git
   ```
3. Instalar dependencias
   ```bash
   npm install
   ```
4. Levantar la api
   ```bash
   npm run start
   ```
5. Ejecutar los test 
   ```bash
   npm run test
   ```