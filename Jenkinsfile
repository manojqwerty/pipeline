pipeline {
  agent any
  tools {
    SONAR_RUNNER_HOME	 'sonar scanner'
    maven 'mvn 3.5.2'
  }
  stages {
       stage('Sonarqube'){
             steps {
             bat 'sonnar-scanner'
               stage('Build') {
                 steps {
                 bat 'mvn clean & mvn package'
                 }
               }
             }
       }
  }   
}
