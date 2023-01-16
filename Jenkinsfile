pipeline {
    agent { 
       dockerfile {
          label "docker"
        }
    }
    stages {
        stage('Test'){
            steps {
                sh 'pip --version'
                sh 'ansible --version'
            }
        }
    }
}
