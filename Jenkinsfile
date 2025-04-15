pipeline {
  agent any

  stages {
    stage('Clonar Repositorio') {
      steps {
        git 'https://github.com/Fabi-daza/techflow.git',branch: 'main'
      }
    }

    stage('Instalar Dependencias') {
      steps {
        sh 'npm install'
      }
    }

    stage('Levantar json-server') {
      steps {
        sh 'npx json-server --watch db.json --port 3000 &'
        sh 'sleep 2'
      }
    }

    stage('Ejecutar Pruebas') {
      steps {
        sh 'npm test'
      }
    }
  }
}
