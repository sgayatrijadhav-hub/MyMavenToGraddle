pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'gradle build'
            }
        }

        stage('Run') {
            steps {
                sh 'java -jar build/libs/MyMavenToGradle-1.0-SNAPSHOT.jar'
            }
        }
    }
}
