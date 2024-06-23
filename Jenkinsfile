pipeline {
    agent {
        label 'slavenode'
                }
    
    stages {
        
        stage('Build') {
            agent{
        label 'slavenode'
                }
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

    }
}
