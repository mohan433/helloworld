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
    stage{'Deployment'){
        steps{
            withmaven(maven: 'maven3.6.3'){
                sh 'mvn deploy'
            }
        }
    }
}                   
