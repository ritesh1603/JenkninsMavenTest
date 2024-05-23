pipeline {
    agent any 
    environment {
        PATH = "C:\\Users\\Shubhada\\Downloads\\apache-maven-3.9.6\\bin;${env.PATH}"
    }
    stages {
        stage('Clean') { 
            steps {
                bat "mvn clean"
            }
        }
        stage('Test') { 
            steps {
                bat "mvn test"
            }
        }
        stage('Deploy') { 
            steps {
                bat "mvn package"
            }
        }
    }
}
