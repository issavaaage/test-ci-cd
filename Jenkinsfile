pipeline {

  agent any

  tools {nodejs "nodejs"}

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
