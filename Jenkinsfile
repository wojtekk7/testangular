pipeline {
  agent any
  
  tools {nodejs "nodejs 14.11.0"}
  
  stages {
    
    stage('Cleanup') {
      steps {
        deleteDir()
       }
    }
    
    
    stage('Install modules') {
      steps {
        bat 'npm install'
       }
    }
    
     stage('Build') {
      steps {
        bat 'npm run-script build'
       }
    }
  }



}
