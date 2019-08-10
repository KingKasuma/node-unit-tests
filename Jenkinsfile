pipeline {
    agent none;
    
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
                    }
                }
            }
        }
        stage('Unit Test') {
            steps{
                script{
                    node{
                        println "Unit Test build"
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
