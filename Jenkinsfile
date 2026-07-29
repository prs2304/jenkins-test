pipeline {
    agent any
    environment {
        DEPLOY = 'staging'
    }
    stages {
        stage('build') {
            when {
                environment name: 'DEPLOY', value: 'production'
            }
            steps {
                echo 'building in production environment'
            }
        }
    }
}
