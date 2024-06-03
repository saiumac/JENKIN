pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout the repository from the main branch
                git url: 'https://github.com/saiumac/JENKIN.git', branch: 'main'
            }
        }
        stage('Build') {
            steps {
                // Install any dependencies if needed
                echo 'No build steps needed for plain HTML'
            }
        }
        stage('Test') {
            steps {
                // Perform any testing if needed
                echo 'No tests defined for plain HTML'
            }
        }
        stage('Deploy') {
            steps {
                sh 'sudo mkdir -p /var/www/html/'

                // Deploy to the server or web server
                sh 'sudo cp -r * /var/www/html/'
            }
        }
    }
}
