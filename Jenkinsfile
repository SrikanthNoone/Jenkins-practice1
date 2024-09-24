pipeline {
    agent { node { label 'Node1' } }

    environment{
        USER = 'sri'
        PASS = '123'
    }

    parallel
     parameters {
        string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')

        text(name: 'BIOGRAPHY', defaultValue: '', description: 'Enter some information about the person')

        booleanParam(name: 'TOGGLE', defaultValue: true, description: 'Toggle this value')

        choice(name: 'CHOICE', choices: ['One', 'Two', 'Three'], description: 'Pick something')

        password(name: 'PASSWORD', defaultValue: 'SECRET', description: 'Enter a password')
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
         stage('Example1') {
            steps {
                echo "Hello ${params.PERSON}"

                echo "Biography: ${params.BIOGRAPHY}"

                echo "Toggle: ${params.TOGGLE}"

                echo "Choice: ${params.CHOICE}"

                echo "Password: ${params.PASSWORD}"
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
        stage("parallel"){
            parallel{
                stage ('testing parallel1111111111'){
                        steps{
                            sh 'sleep 10'
                            echo "parallel running"
                        }
                stage ('testing parallel222222222'){
                        steps{
                            sh 'sleep 10'
                            echo "parallel running"
                        }
                }
            }
        }
        }
    }
}

