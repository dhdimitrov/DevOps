pipeline {
    agent any

    stages {
        stage ('Build') {
            steps {
                sh '''
                    sudo systemctl start httpd
                    sudo systemctl enable httpd
                '''
            }
        }
        stage ('Deploy') {
            steps {
                sh '''
                    sudo cp ./index.html /var/www/html/
                '''
            }
        }
    }
}
