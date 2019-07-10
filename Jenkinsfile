pipeline {
    agent none
    stages {
        stage('Build') {
            agent { docker 'openjdk:8-jdk' }
            steps {
                sh './mvnw -fae verify -Pjava8'
            }
        }
    }
}