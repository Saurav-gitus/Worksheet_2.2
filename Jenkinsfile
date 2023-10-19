pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                // Checkout the code from your Git repository
                bat 'https://github.com/Saurav-gitus/SpringPetClinic.git'
            }
        }
  
        stage('Build') {
            steps {
                // Replace this with your build command (e.g., using Maven)
                bat 'mvn clean install'
            }
        }

        stage('Test') {
            steps {
                // Replace this with your test command (e.g., using Maven)
                bat 'mvn test'
            }
        }

        stage('Deploy') {
            steps {
                // Replace this with your deployment command (e.g., running a script)
                bat 'deploy.bat'
            }
        }
    }
    
    post {
        success {
            // Add post-build actions here (e.g., notifications, archiving artifacts)
        }
    }
}
