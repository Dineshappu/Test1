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

        

        stage('Parallel'){
        Parallel{
        stage('Test1') {
            agent{
        label 'slavenode'
                }
            steps {
                sh '''
                    echo "This is Test stage-1"
                '''
            }
        }

        stage('Test2') {
            agent{
        label 'slavenode'
                }
            steps {
                sh '''
                    echo "This is Test stage-2"
                '''
            }
        }
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
