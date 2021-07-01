def remote = [:]
  remote.name = 'remote'
  remote.host = '172.31.41.17'
  remote.user = 'ubuntu'
  
  
 remote.allowAnyHosts = true  

node {
    withCredentials([sshUserPrivateKey(credentialsId: 'remote-linux', keyFileVariable: 'identity', passphraseVariable: '', usernameVariable: 'ubuntu')]) {
        remote.user = ubuntu
        remote.identityFile = identity
        stage("SSH Steps Rocks!") {
           
            sshCommand remote: remote,sudo: true, command: 'ifconfig'
            
        }
    }
}
