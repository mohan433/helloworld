pipeline{
    agent any
    tools{
        Maven 'maven'
        jdk 'JAVA_11'
     }
    stages{
        stage('Build'){
             steps{
                  bat 'mvn Tests clean package'
  
             }
        }
   }
}    
