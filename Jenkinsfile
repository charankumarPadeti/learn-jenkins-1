pipeline{
    agent {
        node {
            label 'AGENT-1'
        }
    }
    stages{
        stage('Building'){
            steps{
                echo 'Building'
            }
        }
        stage('CHARAN'){
            steps{
                echo 'Test'
            }
        }
        stage('Deploy'){
            steps{
                echo 'Deploy'
            }
        }
    }
    post { 
        always { 
            echo 'I will always say Hello again!'
        }
        success { 
            echo 'Pipeline was successfully done'
        }
        failure { 
            echo 'Pipeline was failure'
        }
    }
}