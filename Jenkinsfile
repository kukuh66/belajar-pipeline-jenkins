pipeline {
    agent {
        node {
            label "linux && java11"
        }
    }

    stages {
        stage('Build') {
            steps {
                echo ('Start build')
                sh('./mvnw clean compile test-compile')
                echo ('Finish build')
            }
        }
        stage('Test') {
            steps {
                echo ('Start test')
                sh('./mvnw test')
                echo ('Finish test')
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