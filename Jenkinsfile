pipeline {
    agent any 

    stages {
        stage('Build Assets') {
            agent any 
            steps {
                echo 'Building vvvvvAssets...'
                chmod +x install.sh
                sh './install.sh'
           }
        }
        
        
        
    }
}
