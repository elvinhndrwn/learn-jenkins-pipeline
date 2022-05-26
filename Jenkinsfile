pipeline{
    agent any
    tools {
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