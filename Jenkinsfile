pipeline {
  agent any
   tools {
    maven 'maven-3.6.3'
  }
  stages {
    stage ('Fetch code') {
      steps {
        git branch: 'paac', url: 'https://github.com/aslanlia/https-github.com-devopshydclub-vprofile-project.git'
      }
    }
    stage('Build') {
      steps {
        sh 'mvn install'  
      }
    } 
    stage('Test') {
      steps {
        sh 'mvn test'
      }
    }
  }
}
