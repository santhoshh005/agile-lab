pipeline{
    agent any
    
    tools{
        maven 'M3'
    }
    
    stages{
        stage('Code Checkout'){
            steps{
                git branch: 'main',
                url: 'https://github.com/santhoshh005/agile-lab.git'
            }
        }
        stage('Build'){
            steps{
                bat 'mvn clean test'
            }
        }
        stage('Install'){
            steps{
                bat 'mvn clean install'
            }
        }
    }
}
