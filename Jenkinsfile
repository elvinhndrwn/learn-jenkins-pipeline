pipeline{
    agent any

    stages{
        stage('Compile'){
            steps{
                withMaven(maven: 'maven_3_8_5'){
                    sh 'mvn clean compile'
                }
            }
        }

        stage('Testing'){
            steps{
                withMaven(maven: 'maven_3_8_5'){
                    sh 'mvn test'
                }
            }
        }

        stage('Deploy'){
            steps{
                withMaven(maven: 'maven_3_8_5'){
                    sh 'mvn deploy'
                }
            }
        }
    }
}