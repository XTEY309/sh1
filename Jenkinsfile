pipeline {
    agent any
    stages {
        stage('git') {
            steps {
                echo "${env.BRANCH_NAME}"  // Используйте правильное имя переменной
            }
        }
        stage('docker Build') {
            steps {
                sh 'docker compose build'  // Убраны лишние скобки и script:
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
