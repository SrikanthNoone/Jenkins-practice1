pipeline {
    agent { node { label 'agent' } }

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
      post { 
        always { 
            echo 'I will always say Hello again!'
        }
        success{
            echo "I will run on success"
        }
        failure{
            echo "I will run on failure"
        }
    }
}