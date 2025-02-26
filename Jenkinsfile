 pipeline {
    agent none
    stages {
     agent ('label node-1')   
     stage('build') {
            steps {
                sh 'ls -lrt ; echo "this is build stage"'
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
        stage('new-stage') {
            steps {
                sh '''
                hostname -i
                echo "this is new-stage"
                '''
            }
        }
    
    }
}

