pipeline {
    agent{
        label 'slavenode'

    stages {
        stage('Build') {
            steps {
                sh '''
                    echo "This is a build stage"
                    sleep 5
                '''
            }
        }

        stage('Test') {
            steps {
                sh '''
                    echo "This is Test stage"
                    sleep 5
                '''
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                    echo "This is Deploy Stage"
                    sleep 5
                '''
            }
        }

        
        }

    }
}
