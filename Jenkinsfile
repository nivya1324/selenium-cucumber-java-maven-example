pipeline {
    agent any
    tools {
        maven 'Maven'
        jdk 'java'
    }
    stages {
        stage ('Initialize') {
            steps {
                sh '''
                    echo "hello"
                    echo "success"
                '''
            }
        }

        stage ('Build') {
            steps {
                sh 'mvn clean verify' 
            }
            post {
                success {
                    junit 'target/surefire-reports/**/*.xml' 
                }
            }
        }
    }
}
