
pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
                git(
                    branch: 'main',
                    url: ''
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
