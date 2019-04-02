node {
   stage('Compile-Package') {
   def mvnHome = tool name:'D:\\softwares\\Windows Softwares\\apache-maven-3.5.2\',type:'maven'
   bat "${mvnHome}/bin/mvn package"
   }
   
   stage ('testing-stage') {
   def mvnHome = tool name:'D:\\softwares\\Windows Softwares\\apache-maven-3.5.2\',type:'maven'
   bat "${mvnHome}/bin/mvn test"
   }
}
   
