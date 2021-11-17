pipeline {
    agent any
    environment {
        PATH="/opt/maven/bin:$PATH"
    }

    stages {
        stage('SCM') {
            steps {
                git 'https://github.com/syedriyaz786/testrepo.git'
            }
        }
        stage('Maven') {
            steps {
               sh "mvn package"
            }
        }
    }     
}   
