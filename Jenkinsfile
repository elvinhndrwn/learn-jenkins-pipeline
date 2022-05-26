pipeline{
    agent any
    tools {
            jdk 'openjdk-1.8'
            maven 'maven_3_8_5'
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