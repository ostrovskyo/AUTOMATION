pipeline {
    agent any

    stages {
        stage('Create project dir') {
            steps {
                sshagent(credentials : ['990b4b0c-f350-448e-bc7e-e60c53e0f400']) {
                sh 'ssh -o StrictHostKeyChecking=no user@hostname.com uptime'
                sh 'ssh -v user@hostname.com'
                sh 'scp ./source/filename user@hostname.com:/remotehost/target'
                }
            }
        }
    }
}
