pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the project...'
                // Replace 'mvn clean package' with the build command for your project.
                sh 'mvn clean package'
            }
        }
    }

    post {
        success {
            echo 'Build was successful!'
        }
        failure {
            echo 'Build failed!'
        }
    }
}
