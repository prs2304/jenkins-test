pipeline {
    agent any
    environment {
        DEPLOY = 'staging'
    }
    stages {
        stage ('build') {
            steps {
                when {
                    environment name: 'DEPLOY', value: 'production'
                }
                step {
                    echo 'building in production environment'
                }
            }
        }
    }
}
