pipeline {
    agent any

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
            agent{
                label 'slavenode'
            }
            steps {
                sh '''
                    echo "This is Test stage"
                    sleep 5
                '''
            }
        }

        stage('Deploy') {
            agent{
                label 'slavenode'
            }
            steps {
                sh '''
                    echo "This is Deploy Stage"
                    sleep 5
                '''
            }
        }

        stage('Test Stage') {
            steps {
                sh '''
                    echo "This is Test Stage"
                    sleep 5
                '''
            }
        }

        
    }
}
