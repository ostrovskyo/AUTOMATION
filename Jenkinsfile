pipeline {
    agent any

    stages {
        stage('Create project dir') {
            steps {
                sshagent(credentials : ['parent_host']) {
                sh 'ssh -o StrictHostKeyChecking=no root@10.0.0.63 uptime'
                }
            }
        }
    }
}
