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
         maven 'maven'
     }
   stages{
        stage('Build'){
             steps{
                  sh 'mvn -B -DskipTests clean package'
             }
        }
   }
}    
