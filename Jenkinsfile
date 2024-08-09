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
                timeout(1) {
                    input message: 'Approve !!! ready to deploy', ok: 'Are you ready to proceed for deployment'
                }
            }
        }
        stage('deploy') {
            steps {
                echo "Deploying ..."
            }
        }
    }
}
