pipeline {
    agent { node { label 'Node1' } }

    environment{
        USER = 'sri'
        PASS = '123'
    }
    
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'pwd'
            }
        }

        stage('example'){
            steps{
                echo 'helllllllllpoooooooooo'
                echo '${USER}'
                echo '${PASS}'
                sh 'printenv'
            }

        }

        
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
                echo "webhook called"
            
            }
        }
    }
}
