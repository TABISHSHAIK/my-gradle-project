
pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/TABISHSHAIK/my-gradle-project.git'
            }
        }

        stage('Build') {
            steps {
                sh './gradlew build'
            }
        }

        stage('Test') {
            steps {
                sh './gradlew test'
            }
        }

        stage('Publish') {
            steps {
                echo 'Publishing to Artifactory...'
                // Add Artifactory upload steps here if configured
            }
        }
    }
}
