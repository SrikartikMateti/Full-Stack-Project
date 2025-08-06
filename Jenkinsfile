  pipeline {
    agent any

    stages {
        stage('Build Backend') {
            steps {
                echo '🔧 Building backend...'
                bat 'type backend\\server.js'
            }
        }

        stage('Build Frontend') {
            steps {
                echo '🎨 Building frontend...'
                bat 'type frontend\\index.html'
            }
        }

        stage('Test') {
            steps {
                echo '✅ Running tests...'
                bat 'echo All dummy tests passed.'
            }
        }

        stage('Deploy') {
            steps {
                echo '🚀 Deploying application (simulated)...'
                bat 'echo Deployment completed.'
            }
        }
    }

    post {
        always {
            echo '📝 Pipeline finished.'
        }
        success {
            echo '🎉 Build was successful!'
        }
        failure {
            echo '❌ Build failed.'
        }
    }
}
