pipeline{
    agent any
    stages{
         stage('maven build'){
            steps{
                tool name: 'Maven', type: 'maven'
                sh 'mvn clean install'
             }
          }
    }  
    stages{
        stage('Git Checkout'){
             steps{   
                  git 'https://github.com/mohan433/helloworld'
            }
        }
    }   
}                   
