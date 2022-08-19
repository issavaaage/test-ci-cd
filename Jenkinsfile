pipeline {

  agent any

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

      }
    }
  }
}
