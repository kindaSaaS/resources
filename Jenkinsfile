pipeline {
    agent any
    
    stages {
        stage('Clone Repository') {
            steps {
                script {
                    // Clean workspace before cloning
                    deleteDir()
                    
                    // Clone the GitHub repository
                    git url: 'https://github.com/facebook/create-react-app.git', branch: 'main'
                }
            }
        }
        
        stage('Install Dependencies') {
            steps {
                script {
                    // Install npm dependencies
                    sh 'npm install'
                }
            }
        }
        
        stage('Build') {
            steps {
                script {
                    // Run npm build command
                    sh 'npm run build'
                }
            }
        }
                stage('hello world') {
            steps {
                script {
                    // Run npm build command
                    sh 'hello world'
                }
            }
        }
    }
}
