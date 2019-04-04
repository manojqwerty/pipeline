pipeline {
  agent any
  tools {
    maven 'mvn 3.5.2'
    java 'jdk1.8'
  }
  stages {
               stage('Build') {
                 steps {
                 bat 'mvn clean & mvn package'
                 }
               }
  }   
}
