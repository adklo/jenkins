pipeline {
    agent { 
        node {
            label 'docker-python'
            }
      }
    triggers {
        pollSCM '* * */2 * *'
    }
    stages {
        stage('Build') {
            steps {
                echo "Building"
                sh '''
                cd myapp
                pip install -r requirements.txt
                '''
            }
        }
        stage('Test') {
            steps {
                echo "Testing..updated
                sh '''
                cd myapp
                python3 hello.py
                python2 hello.py --name=Adrian
                '''
            }
        }
        stage('Deliver') {
            steps {
                echo 'Deliver....'
                sh '''
                echo "doing delivery stuff..update"
                '''
            }
        }
    }

}






