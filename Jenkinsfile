pipeline {
    agent { node { label 'qa' }}
    stages {
        stage('Build') {
            when {
                branch 'develop'
            }
            steps {
                sh 'composer install'
            }
        }
    }
}