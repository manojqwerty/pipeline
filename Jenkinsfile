pipeline {
  agent any
  tools {
    maven 'mvn 3.5.2'
  }
  stages {
       stage('Sonarqube'){
             steps {
             bat 'sonar-scanner'
               stage('Build') {
                 steps {
                 bat 'mvn clean & mvn package'
                 }
               }
             }
       }
  }   
}
