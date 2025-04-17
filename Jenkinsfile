pipeline {
  agent any
  stages {
    stage('Clonar Repositorio') {
      steps {
        git branch: 'main', url: 'https://github.com/Fabi-daza/techflow.git'
      }
    }

    stage('Instalar Dependencias') {
      steps {
        bat 'npm install'
      }
    }

    stage('Levantar json-server') {
      steps {
        bat 'npm run start &'
      }
    }

    stage('Ejecutar Pruebas') {
      steps {
        bat 'npm run test'
      }
    }
  }
}
