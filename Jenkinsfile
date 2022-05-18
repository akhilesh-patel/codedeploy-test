pipeline {
    agent any 

    stages {
        stage('Build Assets') {
            agent any 
            steps {
                echo 'Building Assets...'
            }
        }
        stage('Test') {
            agent any
            steps {
                echo 'Testing stuff...'
                sh 'sudo yum update -y'
                sh 'sudo yum install httpd -y'
                sh 'sudo rm -rf /var/www/html'
                sh 'sudo systemctl start httpd'
                sh 'sudo rm -rf .* && git'
                sh 'sudo git clone https://github.com/akhilesh-patel/awscodedeploy /var/www/html/'
                sh 'sudo systemctl restart httpd'
            }
        }
    }
}
