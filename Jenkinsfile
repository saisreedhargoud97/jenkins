pipeline {
  agent any 
  tools {
    maven 'maven'
  }

  stages {
    stage('compiling') {
      steps {
        sh "mvn compile"
      }
    }

    stage('testing') {
      steps {
        sh "mvn test"
      }
    }
    
    stage('packaging') {
      steps {
        sh "mvn package"
      }
    }

 stage('installing') {
steps {
  sh "mvn install"
}
 }
    stage('site') {
      steps {
        sh "mvn site"
      }
    }
  }
}
   
