pipeline {
    agent any

    stages {
        stage('Checkout code') {
            steps {
                git branch: 'main', url: 'https://github.com/saiumac/JENKIN.git'
            }
        }
        stage('Publish HTML') {
            steps {
                // Assuming your HTML file is located at the root of the repository
                publishHTML reports: 'index.html'
            }
        }
    }
}
