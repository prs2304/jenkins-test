pipeline {
    agent any
    stages {
        stage ('build') {
            steps {
                echo "building the application"
            }
        }
        stage ('building in specific branch') {
            when {
                expression { BRANCH_NAME ==~ /(production|staging)/}
            }
            steps{
                echo "deploying the application"
            }
        }
    }
}
