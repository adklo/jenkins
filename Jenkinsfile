pipeline {
    agent { 
        node {
            label 'docker-python'
            }
      }
    triggers {
        pollSCM '* * * * *'
    }
    stages {
        stage('Build') {
            steps {
                echo "Building.. updated"
                sh '''

                '''
            }
        }
        stage('Test') {
            steps {
                echo "Testing..updated"
                sh '''
                '''
            }
        }
        stage('Deliver') {
            steps {
                echo 'Deliver....'
                sh '''
                echo "doing delivery stuff..update"
                python3 python.py
                '''
            }
        }
    }

}




