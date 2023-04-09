pipeline {
    agent {
        node {
            label "linux && java11"
        }
    }

    stages {
        stage('Hello') {
            steps {
                echo 'Hello Pipeline Test'
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