pipeline{
    agent any
    stages{
        stage('Test'){
                steps{
                       bat 'mvn clean test'
                }
        }

        stage('Build'){
            steps{
                   bat 'mvn -DskipTests=true install'
            }
        }
    }
}