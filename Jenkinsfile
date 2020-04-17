pipeline{
    agent any
    stages{
        stage('Git Checkout'){
             steps{   
                  git 'https://github.com/mohan433/helloworld'
            }
        }
    }
     tools {
         maven 'maven3.6.3'
     }
   stages{
        stage('Build'){
             steps{
                  sh 'mvn -B -DskipTests clean package'
             }
        }
   }
}    
