pipeline {
    agent none;
    
    environment {
        myUsername = "Mike"
    }
    
    stages {
        stage('Test') {
            steps{
                script{
                    node{
                        println "mi primer pipeline"
                    }
                }
            }
        }
        
        stage('Build') {
            steps{
                script{
                    node{
                        println "Build Stage"
                        echo "Nombre de Usuario ${myUsername}"
                    }
                }
            }
        }
        stage('Unit Test') {
            environment{
                myUsername = "Gerald"
            }
            steps{
                script{
                    node{
                        println "Unit Test build"
                        println "Nombre de Usuario $myUsername"
                    }
                }
            }
        }
        stage('Sonar') {
            steps{
                script{
                    node{
                        println "sonar build"
                    }
                }
            }
        }
    }
}
