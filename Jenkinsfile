pipeline{
    agent {
        node {
            label 'AGENT-1'
        }
    }
    environment { 
        GREETING = 'Hello jenkins'
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
                sh """
                    echo "Here i wrote shell script"
                    env
                """
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