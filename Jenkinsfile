pipeline {
    agent {
        dockerfile {
            filename "Dockerfile"
            // args '-p 8989:8989'
            additionalBuildArgs "-t python3-poetry:latest"
        }
    }

    stages {
        stage("Test") {
            steps {
                sh "python --version"
                sh "poetry --version" // this command gets executed inside the container
            }
        }
    }
}
