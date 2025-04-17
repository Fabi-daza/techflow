pipeline {
  agent {
    docker {
      image 'node:18'
    }

  stages {
    stage('Clonar Repositorio') {
      steps {
        git branch: 'main', url: 'https://github.com/Fabi-daza/techflow.git'
      }
    }

    stage('Instalar Dependencias') {
      steps {
        sh 'npm install'
      }
    }

    stage('Levantar json-server') {
      steps {
        sh 'npm run start'
      }
    }

    stage('Ejecutar Pruebas') {
      steps {
        sh 'npm run test'
      }
    }
  }
}
