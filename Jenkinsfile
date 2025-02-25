 pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'ls -lrt; echo "this is build stage"'
            }

        }
        stage('test') {
            steps {
                sh '''
                df -h .
                echo "this is test stage"
                '''
            }

        }
        stage('deploy') {
            steps {
                sh '''
                ps -ef | grep "git"
                echo "this is deploy stage"
                '''
            }
        }    
        stage('my-stage') {
            steps {
                sh '''
                uname -a
                echo "this is my-stage"
                '''
            }
        }
    
    }
}
