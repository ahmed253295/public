pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Clone the repository
                git 'https://github.com/username/my-jenkins-practice.git'
            }
        }
        stage('Run Script') {
            steps {
                // Execute the script
                sh './hello.sh'
            }
        }
    }

    post {
        always {
            echo 'Pipeline execution completed.'
        }
    }
}
