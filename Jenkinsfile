pipeline {
    agent any
    stages {
        stage('Clone Vim repository') {
            steps {
                // Clone the Vim repository to /tmp/vim
                
                sh '''
                echo Starting
                echo brrp
                '''
            }
        }

        stage('Build Vim') {
            steps {
                dir('/var/lib/jenkins/vim') {
                    // Navigate into the vim directory and run the build commands
                    sh '''
			make clean
                        make
                    '''
                }
            }
        }
    }

    post {
        always {
            // Optional: Cleanup the /tmp/vim directory after build
            sh 'echo Finishing'
        }
    }
}