//Declarative pipeline//

pipeline{
    agent any
    stages{
        stage('Checkout SCM'){
            steps{
                sh 'java -version'
            }
        }
        stage('Build'){
            steps{
                sh 'echo mvn build'
            }
        }
        stage('Test'){
            steps{
                sh 'echo mvn test reports'

            }
        }
        stage('Deploy'){
            steps{
                sh 'echo deploying to Dev server'
            }
        }
    }
}
