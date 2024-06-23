pipeline {
    agent {
        label 'slavenode'
    }
    
    stages {
        stage('Build') {
            steps {
                sh '''
                    echo "This is a build stage"
                    sleep 5
                '''
            }
        }

        stage('Parallel') {
            parallel {
                stage('Test1') {
                    steps {
                        sh '''
                            echo "This is Test stage-1"
                        '''
                    }
                }

                stage('Test2') {
                    steps {
                        sh '''
                            echo "This is Test stage-2"
                        '''
                    }
                }
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
