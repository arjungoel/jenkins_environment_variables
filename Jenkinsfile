pipeline {
    agent any
    stage('Deliver for development') {
            when {
                branch 'develop' 
            }
            environment {
                name = 'Arjun'
                job_title = 'Senior AWS DevOps Engineer'
            }
            steps {
                bat "echo My name is ${name}"   
                bat "echo I am working as ${job_title}"
            }
        }
}
