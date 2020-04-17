pipeline{
    agent any
    tools{
        maven 'Maven'
        JAVA 'Java_11'
    } 
    stages{
         stage('Git Checkout'){
             steps{   
                  git 'https://github.com/mohan433/helloworld'
             }
          }
    }  
        stage('maven build'){
            steps{
                tool name: 'Maven', type: 'maven'
            }
        }
}                   
