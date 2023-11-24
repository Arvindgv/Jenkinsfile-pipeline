pipeline{
    
    tools{
        maven 'mymaven'
    }
    
    agent any
    
    stages{
        stage('Clone Repo'){
            steps{
                git 'https://github.com/Sonal0409/DevOpsCodeDemo.git'
            }
        }
        
        stage('Code Review'){
            steps{
                sh 'mvn pmd:pmd'
            }
        }
        
        stage('Test Code'){
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
