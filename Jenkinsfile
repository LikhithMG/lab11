pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
                git(
                    branch: 'main',
                    url: 'https://github.com/LikhithMG/lab11.git'
                )
            }
        }

        stage('Run Shell Script') {
            steps {
                sh '''
                    chmod +x script.sh
                    ./script.sh
                '''
            }
        }

        stage('Run Python Script') {
            steps {
                sh '''
                    python3 script.py
                '''
            }
        }

    }
}
