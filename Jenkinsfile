pipeline {
    agent { node { label 'remote-linux' } }

  stages {  
  stage('Cheking Connection with remote server') {
	      steps {
	          sh 'ifconfig; whoami'
      }
  }

      }
  } 
