
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

        stage('Run Script') {
            steps {
                sh '''
                    chmod +x script.sh
                    ./script.sh
                '''
            }
        }

    }
}
