pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sudo chmod -R 777 ./install_dependencies.sh
                sh './install_dependencies.sh'
            }
        }
    }
}
