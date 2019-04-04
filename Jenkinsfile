pipeline {
  agent any
  tools {
    maven 'mvn 3.5.2'
  }
  stages {
       stage('Sonarqube'){
             steps {
              withSonarQubeEnv('My SonarQube Server') {
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
