pipeline{
    agent any
    
    enivornmnet{
        PATH = "/apache-maven-3.6.3/bin:$PATH"
    }
    stages{
         stage('Git Checkout'){
             steps{   
                  git 'https://github.com/mohan433/helloworld'
             }
          }
        stage('maven build'){
            steps{
                sh "mvn clean package"
     }
}   
