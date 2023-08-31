pipeline {
    agent any
    
    stages {
        stage('Clone Repository') {
            steps {
                script {
                    // Clean workspace before cloning
                    deleteDir()
                    
                    // Clone the GitHub repository
                    git url: 'https://github.com/heroku/node-js-getting-started.git', branch: 'main'
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
                    // Run npm build command (this example doesn't have a build script, so just echoing a message)
                    sh 'echo "Build step"'
                }
            }
        }
    }
}
