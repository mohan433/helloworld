pipeline{
    agent any
    tools{
        maven 'Maven'
        jdk 'Java_11'
    } 
    stages{
        stage('initilize'){
            bat '''
            echo "PATH = %PATH%"
            echo "M2_HOME = %M2_HOME%"
            ...
        }
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
