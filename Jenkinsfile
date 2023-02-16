pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
            sh "ma -C main"
                echo 'Build stage completed'
            }
        }
        stage('Test') {
            steps {
                sh "/var/jenkins_home/workspace/PES1UG20CS196/main/hello_exec"
                echo 'Testing stage completed'
            }
        }
    }
    post {
            failure {
                echo 'Pipeline Failed'
            }
        }
}
