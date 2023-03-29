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
                bat 'rem. .env'
                bat 'echo name=${NAME} >>.env'
                bat 'echo job_title=${JOB} >> .env'
                bat "echo ${name} is working as ${job_title}"
            }
        }
    }
}
