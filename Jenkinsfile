pipeline {
    agent any
    stages{
        stage('STAGE1') {
            steps {
                echo "This is the stage 1"
                echo " Fixed"
            }
        }
        stage('STAGE2') {
            steps {
                sh 'sleep 5'
                echo "This is the stage 2"
            }
        }
        stage('STAGE3') {
            steps {
                echo "This is the stage 3"
                sh '''
                    #!/bin/bash
                    pwd
                    ls -lrt
                    sleep 10
                '''
            }
        }
    }
}