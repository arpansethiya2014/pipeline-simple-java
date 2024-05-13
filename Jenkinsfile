pipeline {
    agent any
    
 environment{

            VERSION_NAME="1.34"
 }

    stages {
        stage("compile") {
            steps {
                echo "javac Main.java"
                echo "${VERSION_NAME}"
            }
        }
        
       stage("run") {
            steps {
                echo "java Main"
           }
        }
        }

 post{

        always {

            echo "always"
        }

        success{
            echo "success"
        }

        failure{
            echo "failure"
        }

    }

}
