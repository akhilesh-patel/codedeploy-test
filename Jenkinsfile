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
            }
        }
    }
}
