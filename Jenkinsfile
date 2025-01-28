pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git 'https://github.com/Dimonde85/juice-shop'
            }
        }

        stage('Print Dockerfile Content') {
            steps {
                script {
                    def dockerfileContent = readFile('Dockerfile')
                    echo "Dockerfile Content: "
                    echo dockerfileContent
                }
            }
        }
    }
}
