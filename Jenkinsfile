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

    stage('Ejecutar Pruebas') {
      steps {
        bat 'npm run test'
      }
    }
  }
}
