//Declarative pipeline//

pipeline{
    agent any
    stages{
        stage('Checkout SCM'){
            steps{
                git url: 'https://github.com/salvadihari/hps-repo.git'
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
        stage('Example') {
            steps {
                echo "Running job # ${env.BUILD_ID} on ${env.JENKINS_URL} server"
            }
        }
    }
}
