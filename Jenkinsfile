pipeline {
    agent { node { label 'Node1' } }
    environment{

        USER = 'srikanth'
        pass = '123'
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'pwd'
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
