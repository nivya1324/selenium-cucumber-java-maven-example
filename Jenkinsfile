pipeline {
    agent any
    tools {
        maven 'Maven'
        jdk 'java'
    }
    stages {
        stage ('Initialize') {
            steps {
                
                    echo "hello"
             
            }
        }

        stage ('Build') {
            steps {
                echo "hello"
            }
            post {
                success {
                    junit 'target/surefire-reports/**/*.xml' 
                }
            }
        }
    }
}
