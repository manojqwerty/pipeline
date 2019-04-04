pipeline {
  agent any
  tools {
    maven 'mvn 3.5.2'
  }
  stages {
    stage('Build') {
      steps {
        bat 'mvnclean mvn package'
      }
    }
  }
}   
