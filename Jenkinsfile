pipeline {
    agent any 

    stages {
        stage('Build Assets') {
            agent any 
            steps {
                echo 'Building Assets...'
               sh './install.sh'
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
