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
                
            }
            post {
                success {
                    junit 'target/surefire-reports/**/*.xml' 
                }
            }
        }
    }
}
