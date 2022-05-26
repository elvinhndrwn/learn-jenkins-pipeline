pipeline{
    agent any
    tools {
            jdk 'openjdk-1.8'
            maven 'Maven_3_5_2'
        }

    stages{
        stage('Compile'){
            steps{
                sh 'mvn clean compile'
            }
        }

        stage('Testing'){
            steps{
                sh 'mvn test'
            }
        }

        stage('Deploy'){
            steps{
                sh 'mvn deploy'
            }
        }
    }
}