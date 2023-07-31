pipeline{
    tools{
        jdk 'JAVA_HOME'
        maven 'M2'
    }
    agent any
    stages{
        stage("checkout"){
            steps{
                git 'https://github.com/AMAR435649/mvn_jenkins-pipeline.git'
            }
        }
        stage("compile"){
            steps{
                sh 'mvn compile'
            }
        }
        stage("test"){
            steps{
                sh 'mvn test'
            }
        }
        stage("package"){
            steps{
                sh 'mvn package'
            }
        }
        stage("deploy"){
            steps{
                sh 'deploy my application'
            }
        }
    }
}

