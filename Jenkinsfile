pipeline {

  agent any

  tools {
    nodejs '18.7.0g'
  }

  stages {
    stage("build") {
      steps {
        sh 'npm install'
        sh 'npm build --prod'
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
