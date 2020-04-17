pipeline {
    agent any
    stage {
         stage ('Git Checkout'){
             steps{   
                  git 'https://github.com/mohan433/helloworld'
      // Get maven home path
      def mavenhome = tool name: 'Maven', type: 'maven'
      def javahome = tool  name: 'JAVA_11', type: 'jdk'
      sh "${mavenhome}/bin/mvn package"
    }
 }   
