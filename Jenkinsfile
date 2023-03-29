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
                bat "echo ${name} is working as ${job_title}"
            }
        }
    }
}
