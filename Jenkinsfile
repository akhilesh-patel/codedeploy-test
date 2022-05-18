pipeline {
    agent any 

    stages {
        stage('Build Assets') {
            agent any 
            steps {
                echo 'Building Assets...'
                sudo sh 'scripts/stop_server.sh'
                sudo  sh 'scripts/after_install.sh'
                sudo sh 'scripts/install_dependencies.sh'
                sudo sh 'scripts/start_server.sh'
                sudo sh 'scripts/validate_service.sh'
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
