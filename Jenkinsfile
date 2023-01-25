pipeline {
    agent any
    environment {
        AAA_SECRET_TEXT = credentials('secret-text')
    }
    stages {
        stage('hello') {
            steps {
                sh 'touch .env'
                sh 'echo $AAA_SECRET_TEXT > .env'                
            }
        }
    }
}