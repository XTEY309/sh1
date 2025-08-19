pipeline {
    agent any
    stages {
        stage('git') {
            steps {
                echo '$GIT_branch'
            }
        }
        stage('docker Build') {
            steps {
                sh(script: 'docker compose build')
            }
        }
        stage('Ok') {
            steps {
                sleep 5 
                echo 'I\'m ok'
                }
            }
        }
}
