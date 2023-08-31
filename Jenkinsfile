pipeline {
    agent any
    
    stages {
        stage('Clone Repository') {
            steps {
                script {ערקע
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
    }
}
