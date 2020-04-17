pipeline {
  agent any
  stage ('SCM checkout'){
    git "https://github.com/mohan433/helloworld"
    }
    stage ('compile-package'){
      // Get maven home path
      def mavenhome = tool name: 'Maven', type: 'maven'
      sh "${mavenhome}/bin/mvn package"
    }
 }   
