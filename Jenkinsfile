pipeline {
    agent {
        node {
            label "linux && java11"
        }
    }

    stages {
        stage('Build') {
            steps {
                echo 'Step for build'
            }
        }
        stage('Test') {
            steps {
                echo 'step for test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Hello Pipeline Deploy'
            }
        }
    }

    post {
        always {
            echo "Always Hello"
        }
        success {
            echo "Build Succes"
        }
        failure {
            ehco "Oh no, Failure"
        }
        cleanup {
            echo "Dont care success"
        }
    }
}