pipeline {
    agent { node { label 'Node1' } }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
               echo 'hello github webhook'
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
            }
        }
    }
}
