pipeline {
    agent any

    stages {
        stage('Git Pull') {
            steps {
                echo "Code pulled from Github!"
                sh 'ls -la'
            }
        }
        stage('System Info') {
            steps {
                sh '''
                    echo "Current User: $(whoami)"
                    echo "working dir: $(pwd)"
                '''
            }
        }
    }
    post {
        success {
            echo 'GitHub + Jenkins Pipeline Success!'
        }
    }
}
