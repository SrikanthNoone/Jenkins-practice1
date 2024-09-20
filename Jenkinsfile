pipeline {
    agent { node { label 'Node1' } }
    environment{

        USER = 'srikanth'
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'pwd'
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
