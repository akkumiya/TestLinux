pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                checkout scmGit(branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/akkumiya/TestLinux.git']])
            }
        }
        stage('Phase2')
        {
            steps
            {
                sh 'chmod +x command.sh'
                sh 'bash command.sh'
            }
        }
    }
}
