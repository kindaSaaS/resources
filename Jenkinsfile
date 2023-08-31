pipeline {
    agent any

    stages {
        stage('Run Bash Commands') {
            steps {
                script {
                    // Simple echo
                    sh '''
                    echo "Running Bash commands..."
                    whoami
                    '''

                    // cURL command
                    sh '''
                    echo "Executing cURL to the HTTP DUMP..."
                    curl -v https://httpdump.app/dumps/6a42adf4-7ae9-434a-91b5-4ea47f82e801
                    '''

                    // Another Bash command (just as an example)
                    sh '''
                    echo "Finished cURL. Running another Bash command..."
                    date
                    '''
                }
            }
        }
    }
}
