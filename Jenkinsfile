pipeline{
    agent {
     label 'Master'
    }
    stages {
        stage('Checkout'){
            checkout scm
       }
        stage ('Dependencies'){
            steps{
                sh 'npm --version'
                echo 'Installed dependencies'
            }
        }   
        stage ('build'){
            steps{
                echo 'Build completed'
            }
        }
        stage ('test'){
            steps{
                echo 'Test Completed'
            }
        }
        stage ('deploy'){
             steps{
                 echo 'Deploy Completed'
             }   
        }
    }
}
