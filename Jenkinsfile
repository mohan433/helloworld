pipeline{
    agent any
    tools {
         tool name: 'Maven', type: 'maven'
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
