pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
                echo 'Repository cloned successfully!'
            }
        }

        stage('Build') {
            steps {
                echo 'Building Project...'
            }
        }

        stage('Run Python') {
            steps {
                bat 'python app.py'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing Completed'
            }
        }
    }

    post {
        always {
            echo 'Pipeline Finished'
        }

        success {
            echo 'Build Successful'
        }

        failure {
            echo 'Build Failed'
        }
    }
}
