pipeline {
    agent any
    stages {
        stage('Compile') {
            steps{
                bat 'Done'
            }
        }
    }
    post {
        failure {
            mail bcc: '', body: "$BUILD_NUMBER", subject: "$JOB_NAME", to: 'aharini545@gmail.com'
        }
        success {
            mail bcc: '', body: "$BUILD_NUMBER", subject: "$JOB_NAME", to: 'aharini545@gmail.com'
        }      
    }
}
