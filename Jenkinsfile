#!groovy
pipeline {
    agent none
   stages {     
    stage('Maven Install') {
      environment { HOME = "${env.WORKSPACE}" }
      agent {         
       docker {          
         image 'maven:3.5.0'         
     }       
  }       
  steps {
       sh 'mvn clean install'
       }
     }
   }
 }