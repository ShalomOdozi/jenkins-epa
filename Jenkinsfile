pipeline {
    agent none 
    stages {
        stage('Test'){
            agent{ dockerfile true }
            steps {
                sh 'pip --version'
                sh 'ansible --version'
            }
        }
    }
}
