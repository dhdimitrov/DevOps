pipeline {
    agent any

    stages {
        stage ('Build') {
            steps {
                sh '''echo "This is Build Stage"'''
            }
        }
        stage ('Test') {
            steps {
                sh '''echo "This is Test Stage"'''
            }
        }
        stage ('Deploy') {
            steps {
                sh '''sudo sh ./script.sh'''
            }
        }
    }
}
