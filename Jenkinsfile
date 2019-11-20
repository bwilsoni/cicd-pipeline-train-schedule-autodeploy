pipeline {
    agent any
    environment {
        DOCKER_IMAGE_NAME = "bwilsoni/train-schedule"
    }
    stages {
        stage('Do Stuff') {
            steps{
                echo 'Running first step in Do Stuff build stage'
                echo 'Actually do some more stuff here first'
            }
        }
        stage('More Cool Things') {
            steps {
                echo 'Wow, more neat things are happening'
            }
        }
    }
}