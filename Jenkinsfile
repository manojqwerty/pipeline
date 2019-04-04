pipeline {
  agent any
  tools {
    maven 'mvn 3.5.2'
  }
  stages {
       stage('Sonarqube'){
             steps {
              withSonarQubeEnv('my sonar server') {
                bat 'sonar:sonar'
               stage('Build') {
                 steps {
                 bat 'mvn clean & mvn package'
                 }
               }
             }
           }
       }
  }   
}
