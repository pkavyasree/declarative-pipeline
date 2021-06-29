pipeline {
    agent any

  stages {  
  stage('Cheking Connection with remote server') {
      agent { label 'remote-linux' }
      steps{
    sshCommand remote: remote, command: "ifconfig; whoami"
      }
  }

      }
  }
