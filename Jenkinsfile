pipeline{
    agent {
     label 'Master'
    }
    stages {
        stage('Checkout'){
            steps{
            checkout scm
            }
        }
        stage ('Dependencies'){
            steps{
                sh 'npm --version'
                echo 'Installed dependencies'
            }
        }   
        stage ('build'){
            steps{
                sh 'npm start'
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
