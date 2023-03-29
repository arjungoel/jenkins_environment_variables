pipeline {
    agent any 
    stages {
        stage('develop') {
            when {
                branch 'develop'
            }
            environment {
                name = 'Arjun'
                job_title = 'Senior AWS DevOps Engineer'
            }
            steps {
                bat 'New-Item .env'
                bat 'echo name=${name} >>.env'
                bat 'echo job_title=${job_title} >> .env'
                bat "echo ${name} is working as ${job_title}"
            }
        }
    }
}
