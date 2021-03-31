pipeline {
    agent any
    environment {
        PATH= "/opt/apache-maven-3.6.3/bin/:$PATH"
    }
    stages {
        stage('clone code') {
            steps {
                git 'https://github.com/kishoregardas/hello-world-war.git'
            }
        }
        stage('build') {
            steps {
                sh "mvn clean package"
            }
        }
    }
}
