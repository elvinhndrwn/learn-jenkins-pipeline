pipeline{
    agent any
    tools{
        tool name: 'maven_3_8_5', type: 'maven'
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