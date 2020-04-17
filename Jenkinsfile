pipeline{
    agent any
    tools {
        Maven : 'maven'
        JAVA_11 : 'jdk'
     }
    stages{
        stage('Git Checkout'){
             steps{   
                  git 'https://github.com/mohan433/helloworld'
            }
        }
    }
  stages{
        stage('Build'){
             steps{
                  sh 'mvn -B -DskipTests clean package'
             }
        }
   }
}    
