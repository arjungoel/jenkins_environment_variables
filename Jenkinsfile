pipeline {
    agent any 
    stages {
        stage('develop') {
            when {
                branch 'develop'
            }
            environment {
                NAME = 'Arjun'
                JOB = 'Senior AWS DevOps Engineer'
            }
            steps {
                bat 'rm .env'
                bat 'rem. .env'
                bat "echo NAME=${NAME} >>.env"
                bat "echo JOB=${JOB} >> .env"
                bat "echo ${name} is working as ${job_title}"
            }
        }
    }
}
