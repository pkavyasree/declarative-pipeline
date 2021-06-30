def remote = [:]
  remote.name = 'remote'
  remote.host = '65.0.89.176'
pipeline {
    agent { node { label 'remote-linux' } }

  stages {  
  stage('Cheking Connection with remote server') {
	      steps {
       sshCommand remote: remote, command: "ifconfig; whoami"
      }
  }

      }
  } 

