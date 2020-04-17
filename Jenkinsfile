pipeline{
    agent any
    
    tools{
        Maven = 'tool name: 'Maven', type: 'maven'
        JAVA = 'tool name: 'JAVA_11', type: 'jdk'
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
    }
    stage{'Deployment stage'){
        steps{
            withmaven(maven: 'maven3.6.3'){
                sh 'mvn deploy'
            }
        }
    }
}                   
