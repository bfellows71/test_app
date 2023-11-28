pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    echo 'Building Flutter app'
                    sh 'flutter pub get'
                    sh 'flutter build apk'
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
