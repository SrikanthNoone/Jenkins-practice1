pipeline {
    agent { node { label 'Node1' } }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
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
    post{
        always{
            echo "i will always run"
           }
      failure{
          echo "i will run on failure"
           }
         }
}
