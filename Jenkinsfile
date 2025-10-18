pipeline {
    agent any

    stages {
        stage('Run tests') {
            steps {
                sh 'node app.js'
            }
        }
    }

    post {
        success {
            echo '✅ Build and tests passed successfully!'
        }
        failure {
            echo '❌ Build or tests failed.'
        }
    }
}
