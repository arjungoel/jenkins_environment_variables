pipeline {
    agent any
    environment {
        AAA_SECRET_TEXT = credentials('secret-text')
        name = 'Arjun'
        job_title = 'Senior AWS DevOps Engineer'
    }
    stages {
        stage('hello') {
            steps {
                bat 'echo $AAA_SECRET_TEXT'     
                bat "echo My name is ${name}"   
                bat "echo I am working as a ${job_title}"
                sh 'printenv'
            }
        }
    }
}
