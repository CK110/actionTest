pipeline {
    agent { label 'master' }
    environment {
        mailer = 'chenkaic4233@gmail.com' 
    }
    stages {
        stage('Example') {
            steps {
                echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}  ${env.mailer}"
            }
        }
    }
    post{
        always{
            sendEmail('chenkaic4233@gmail.com')
        }
    }
}
