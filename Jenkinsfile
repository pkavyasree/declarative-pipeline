pipeline {

    agent {
        node {
            label 'remote-linux'
        }
    }
    stages {  
	 
       stage('Cheking Connection with remote server') {
       steps{
       sshCommand remote: remote, command: "ifconfig; whoami"
      }
  }

      }
  } 
