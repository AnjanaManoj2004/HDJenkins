pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                // If you want to copy files to a dist folder or perform other build steps
                script {
                    // Create a build directory (dist)
                    sh 'mkdir -p dist'
                    // Copy all files to the dist directory
                    sh 'cp -r * dist/' // Copy all files to the dist folder
                    
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
