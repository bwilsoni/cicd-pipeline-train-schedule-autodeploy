pipeline {
    agent any
    environment {
        DOCKER_IMAGE_NAME = "bwilsoni/train-schedule"
    }
    stages {
        stage('Build') {
            when {
                branch 'dev'
            }
            steps {
                echo 'Neat stuff here'
                echo "Docker image name: $DOCKER_IMAGE_NAME"
            }
        }
    }
}