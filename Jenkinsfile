pipeline {
    agent any
    stage {
    git "https://github.com/mohan433/helloworld"
    }
    stage ('compile-package'){
      // Get maven home path
      def mavenhome = tool name: 'Maven', type: 'maven'
      def javahome = tool  name: 'JAVA_11', type: 'jdk'
      sh "${mavenhome}/bin/mvn package"
    }
 }   
