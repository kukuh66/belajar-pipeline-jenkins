pipeline {
    agent {
        node {
            label "linux && java11"
        }
    }

    stages {
        stage('Build') {
            steps {
                echo ('Step for build')
                sleep (5)
                echo ('Step for build2')
            }
        }
        stage('Test') {
            steps {
                echo ('step for test')
                sleep (10)
                echo ('step for test 2')
            }
        }
        stage('Deploy') {
            steps {
                echo ('Hello Pipeline Deploy')
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