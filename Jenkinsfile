pipeline {
    agent any
    triggers {
        pollSCM '* * * * *'
    }
    stages {
        stage('Build') {
            steps {
                echo "Building2.."
            }
        }
        stage('Test') {
            steps {
                echo "Testing2.."
            }
        }
        stage('Deliver') {
            steps {
                echo 'Deliver2....'
            }
        }
    }
}