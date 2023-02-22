pipeline {
    agent any
    stages {
        stage('ssh') {
            step([$class: 'WsCleanup'])
            steps {
                script{
                     
                 
                   
                  
                  
                   
                         
 
                  // Copy file to remote server 
                  sshPublisher(publishers: [sshPublisherDesc(configName: 'ansible',
                    transfers: [ sshTransfer(flatten: false,
                                 remoteDirectory: '',
                                             sourceFiles: '. *'
                    )])
                  ])
                   
                  
                     
                }
            }
        }
    }
         
}
