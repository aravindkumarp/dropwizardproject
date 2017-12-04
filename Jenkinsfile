pipeline {
    agent any
   stages {
        stage('build') {
            steps {
                echo "The build stage"
            }
        }
         stage('test') {
            steps {
                echo "The test stage"
            }
        }
         stage('deploy') {
            steps {
                echo "The deploy stage"
            }
        }
    }
    post {
        always {
            echo 'Stages have completed'
        }
        success {
            echo 'successful'
        }
        failure {
            echo 'failed'
        }
        unstable {
            echo 'marked as unstable'
        }
        changed {
            echo 'This will run only if the state of the Pipeline has changed'
            echo 'For example, if the Pipeline was previously failing but is now successful'
        }
    }
}
