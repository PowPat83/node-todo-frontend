pipeline {
  agent any
    
  tools {nodejs "npm"}
    
  stages {
        
    stage('Cloning Git') {
      steps {
        git 'https://github.com/powpat83/node-todo-frontend'
      }
    }
        
    stage('Install dependencies') {
      steps {
        sh 'npm install'
      }
    }
     
    stage('Test') {
      steps {
         sh 'npm test'
      }
    }      
  }
}
