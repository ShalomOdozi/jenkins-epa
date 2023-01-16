pipeline {
    agent none 
    stages {
      stage("Checkout"){
        agent{
            label "Linux"
        }
        steps{
            git(
                url: 'git@github.com:ShalomOdozi/jenkins-epa.git',
                branch: "main"
            )
        }
      }
      stage('Build'){
        agent { 
            dockerfile {
            filename 'Dockerfile'
            label 'Linux'
            args "-v /home/user/jenkin:/var/jenkin" 
        }
      }
        steps {
            sh 'pip --version'
            sh 'ansible --version'
            }
        }
    }
}
