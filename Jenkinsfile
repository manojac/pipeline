pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'sleep 5; echo "this is build stage"'
            }

        }
        stage( 'test') {
            steps {
                '''
                sleep 5
                echo "this is test stage"
                '''
            }

        }
        stage( 'deploy') {
            steps {
                '''
                sleep 5
                echo "this is deploy stage"
                '''
            }

        stage( 'my-stage') {
            steps {
                '''
                sleep 5
                echo "this is my-stage"
                '''
            }
        }
        }
    
    }
}
