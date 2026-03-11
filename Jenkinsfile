pipeline {
    agent any

    stages {

        stage('Clone Repository') {
            steps {
                git branch: 'main', url: 'https://github.com/geet1289dev/my-website.git'
            }
        }

        stage('Deploy Website') {
            steps {
                sh '''
                sudo cp -r * /usr/share/nginx/html/
                '''
            }
        }

    }
}
