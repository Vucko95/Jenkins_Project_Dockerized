#!groovy

pipeline {
    agent any

    tools {
        maven "3.8.5" 
    }

    stages {
        stage("Build") {
            steps {
                git 'https://github.com/Vucko95/Jenkins_Dockerized_Project.git'
                // sh "mvn clean install"
                sh "mvn -f /var/tiger_project/pom.xml clean install"
            }
        }
    }

    // post {
    //     always {
    //         cleanWs()
    //     }
    // }
}


