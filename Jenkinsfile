pipeline {
    agent any
    fsf
    stages {
        stage('Clone Repository') {
            steps {
                script {
                    // Clean workspace before cloning
                    deleteDir()
                    
                    // Clone the GitHub repository
                    git url: 'https://github.com/heroku/node-js-sample.git', branch: 'main'
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
    }
}
