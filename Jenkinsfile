pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'sudo -S docker build -t ${JOB_NAME}-${BUILD_NUMBER} . && sudo -S python3 -m pip3 install --upgrade pip'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}