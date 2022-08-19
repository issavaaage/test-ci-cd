pipeline {

  agent any

  tools {
    nodejs '14.17.5'
  }

  stages {
    stage("build") {
      steps {
        sh 'npm install'
        sh 'npm install -g @angular/cli@12.2.18'
        sh 'ng build --prod'
      }
    }
    stage("test") {
      steps {
        sh 'ng test'
      }
    }
    stage("deploy") {
      steps {
        echo "deploy"
      }
    }
  }
}
