pipeline {
    agent { node { label 'Node1' } }
    
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
