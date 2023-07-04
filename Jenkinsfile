pipeline {
    agent any

    stages {
        stage ('Build') {
            steps {
                sh '''
                    sudo yum update -y
                    sudo yum install -y httpd
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
