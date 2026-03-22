pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'chmod +x gradlew'
                sh './gradlew build --no-daemon'
            }
        }

        stage('Run') {
            steps {
                sh 'java -jar build/libs/*.jar'
            }
        }
    }
}
