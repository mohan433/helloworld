pipeline{
    agent any
    tools{
        maven 'Maven'
        jdk 'JAVA_11'
    }
    stages{
        stage('Build'){
             steps{
                  bat 'mvn test clean package'
  
             }
        }
   }
}    
