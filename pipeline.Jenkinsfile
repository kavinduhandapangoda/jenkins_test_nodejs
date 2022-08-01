pipeline{
    agent any
    tools{nodejs "NodeJS"}
    stages{
        stage('Build'){
            steps{
                git branch: 'main', url: 'https://github.com/kavinduhandapangoda/jenkins_test_nodejs.git'
                bat 'npm install'
            }
        }
        stage('Run'){
            steps{
                bat 'node index.js'
            }
        }
    }
}
