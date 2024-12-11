pipeline {
    agent any  
    stages {
        stage('Clone Repository') {
            steps {
                echo 'Cloning the repository...'
                git branch: 'main', url: 'https://github.com/vit-zeeshan/Youtube-Clone.git'
            }
        }
        stage('Build') {
            steps {
                echo 'Building the project...'
                // Add your build commands here
                sh 'echo Build successful!'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                // Add your test commands here
                sh 'echo Tests passed!'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying the project...'
                // Add your deployment commands here
                sh 'echo Deployment successful!'
            }
        }
    }

    post {
        always {
            echo 'Cleaning up...'
        }
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed. Check logs.'
        }
    }
}
