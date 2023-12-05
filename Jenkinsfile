pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    echo 'Building Flutter app'
                    sh 'flutter clean'
                    sh 'flutter build apk --split-per-abi'
                }
            }
        }
        stage('Test') {
            steps {
                script {
                    echo 'Running Flutter tests'
                    sh 'flutter test'
                }
            }
        }
    }
}
