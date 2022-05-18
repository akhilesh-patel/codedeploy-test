pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
             sh "chmod +x -R ${env./var/lib/jenkins/workspace/pipe-line-2}"
             sh  './install_dependencies.sh'
               

             
            }
        }
    }
}
