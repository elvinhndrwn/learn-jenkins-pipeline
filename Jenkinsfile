pipeline{
    agent any
    tools{
        tool name: 'maven_3_8_5', type: 'maven'
    }

    stages{
        stage('Build'){
            steps{
                   bat 'mvn clean install'
            }
        }
    }
}