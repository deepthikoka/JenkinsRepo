pipeline{
    
    tools{
        maven 'MyMaven'
    }
    
    agent any
    
    stages{
        stage ('Clone a repo') {
            steps{
                git 'https://github.com/Sonal0409/DevOpsCodeDemo.git'
            }
        }
        stage('Compile Code') {
            steps{
                sh 'mvn compile'
            }
        }
        stage('Test code'){
            steps{
                sh 'mvn test'
            }
        }
        stage('Package'){
            steps{
                sh 'mvn package'
            }
        }
   
    }
    
}
