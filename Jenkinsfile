pipeline {
    agent any 

    stages {
        stage('Build Assets') {
            agent any 
            steps {
                echo 'Building Assets...'
                sh 'scripts/stop_server.sh'
                sh 'scripts/after_install.sh'
                sh 'scripts/install_dependencies.sh'
                sh 'scripts/start_server.sh'
                sh 'scripts/validate_service.sh'
            }
        }
        stage('Test') {
            agent any
            steps {
                echo 'Testing stuff...'
            }
        }
        
        
        stage('deploy') {
            agent any
            steps {
                echo 'deploy...'
            }
        }
        
        
    }
}
