pipeline {
    agent any
    
    stages {
        stage("compile") {
            steps {
                echo "java .\Main.java"
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
