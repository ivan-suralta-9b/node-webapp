pipeline {
  agent {
    label 'linux-node'
  } 
  stages {
    stage("Build &  Run") {
      steps {
        script {
          docker.build('node-webapp').run('-p 3000:3000') 
        }
      }
    }
  }
}
