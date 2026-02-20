pipeline {
    agent any

    stages {
        stage('Clone Repo') {
            steps {
                git branch: 'main', url: 'https://github.com/Shruti-S-Prajapati/ml-cicd-project.git'
            }
        }
        
        stage('Install Dependencies') {
            steps {
                bat 'pip install -r requirements.txt'
            }
        }
        
        stage('Run Training') {
            steps {
                bat 'python train.py'
            }
        }
    }
}
