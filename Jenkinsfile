pipeline {
    agent any
    environment {
        AAA_SECRET_TEXT = credentials('secret-text')
    }
    stages {
        stage('hello') {
            steps {
                bat 'echo $AAA_SECRET_TEXT'     
                bat 'echo My name is ${name}'   
                bat 'echo I am working as a ${job_title}'
            }
        }
    }
}
