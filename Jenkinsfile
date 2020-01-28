pipeline {
    agent {
        docker { image 'docker-artifacts.twt-dh.de/android-box' }
    }
    stages {
        stage('Build') {
            steps {
                sh './gradlew clean && ./gradlew assembleRelease'
            }
        }
    }
}