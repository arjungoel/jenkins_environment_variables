pipeline {
    agent any
    environment {
        AAA_SECRET_TEXT = credentials('secret-text')
    }
    stages {
        stage('hello') {
            steps {
                bat 'touch .env'
                bat 'echo $AAA_SECRET_TEXT > .env'                
            }
        }
    }
}