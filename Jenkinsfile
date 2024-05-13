pipeline {
    agent any
    
    stages {
        stage("Compile") {
            steps {
                sh 'javac Main.java'
            }
        }
        
        stage("Run") {
            steps {
                sh 'java Main'
            }
        }
    }
    
    post {
        always {
            echo "Post-Build: Always executed"
        }
        success {
            echo "Post-Build: Successfully executed"
        }
        failure {
            echo "Post-Build: Failed execution"
        }
    }
}
