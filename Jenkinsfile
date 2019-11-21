pipeline {
    agent any
    environment {
        DOCKER_IMAGE_NAME = "bwilsoni/train-schedule"
    }
    stages {
        stage('Build') {
            when {
                anyOf {
                    branch 'dev'
                    branch 'master'
                }
            }
            steps {
                echo 'Running build automation'
                sh './gradlew build --no-daemon'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
}