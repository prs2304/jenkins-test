pipeline {
    agent any
    environment {
        DEPLOY = 'production'
    }
    stages {
        stage ('build') {
            steps {
                echo "deploy to the ${DEPLOY}"
            }
        }
    }
}
