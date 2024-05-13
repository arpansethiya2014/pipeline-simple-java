pipeline{

    agent any 
    stages{
        

        stage("compile"){
               
            steps{
                   sh 'javac Main.java'
            }

        }

        stage("run"){

           steps{
             sh "java Main"
           }

        }
    }

    post{

        always {

            sh 'echo "always"'
        }

        success{
            sh 'echo "success"'
        }

        failure{
            sh 'echo "failure"'
        }

    }

}