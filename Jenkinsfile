pipeline{
    agent any
    stages{
         stage('Git Checkout'){
             steps{   
                  git 'https://github.com/mohan433/helloworld'
             }
          }
    }  
        stage('maven build'){
            steps{
                sh "mvn clean package"
            }
        }
}                   
