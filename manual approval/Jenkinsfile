pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                echo "Building ..."
            }
        }
        stage('Approval') {
            steps {
                input 'Approve !!! ready to deploy'
            }
        }
        stage('deploy') {
            steps {
                echo "Deploying ..."
            }
        }
    }
}
