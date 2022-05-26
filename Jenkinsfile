pipeline{
    agent any

    stages{
        stage('Test'){
            steps{
                sh 'nohup ./mvnw clean install'
            }
        }
    }
}