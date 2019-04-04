pipeline {
  agent any
  tools {
    maven 'mvn 3.5.2'
    java 'jdk 1.8'
  }
  stages {
               stage('Build') {
                 steps {
                 bat 'mvn clean & mvn package'
                 }
               }
  }   
}
