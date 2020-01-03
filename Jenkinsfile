// Declarative Pipeline
pipeline {
    agent {label 'master'}
    stages {
        stage('Source') { // Get code
            steps {
                // get code from our Git repository
                git 'https://github.com/saianuragreddy/spring3-mvc-maven-xml-hello-world.git'
            }
        }
        stage('Compile') { // Compile and do unit testing
            steps {
                // run Gradle to execute compile and unit testing
                sh "maven package"
            }
        }
    }
}