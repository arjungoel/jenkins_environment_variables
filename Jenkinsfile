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
                bat 'del .env'
                bat 'rem. .env'
                bat "echo NAME=${NAME} >>.env"
                bat "echo JOB=${JOB} >> .env"
                bat "echo ${name} is working as ${job_title}"
            }
        }
        stage('master') {
            when {
                branch 'main'
            }
            environment {
                NAME = 'Harsh Goel'
                JOB = 'Senior Data Engineer'
                COMPANY = 'XYZ'
            }
            steps {
                bat 'del .env'
                bat 'rem. .env'
                bat "echo NAME=${NAME} >>.env"
                bat "echo JOB=${JOB} >> .env"
                bat "echo COMPANY=${COMPANY} >> .env"
                bat "echo ${name} is working as ${job_title} for ${COMPANY}"
            }
        }
    }
}