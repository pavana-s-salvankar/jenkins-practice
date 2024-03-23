@Library("shared-library") _
pipeline {
    agent any
    triggers {
        pollSCM '* * * * *'
    }
    stages {
        stage ('Starting seedjob') {
        build job: 'seedjob'
}
        stage('Build') {
            steps {
                echo "Building.."
            }
        }
        stage('Test') {
            steps {
                echo "Testing.."
            }
        }
        stage('Deliver') {
            steps {
                echo 'Deliver....'
                printSuccess()
            }
        }
    }
}
