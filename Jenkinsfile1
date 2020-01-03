// Scripted Pipeline
node('master') {
    stage('Source') { // Get code
        // get code from our Git repository
        git credentialsId: 'e573c0a6-8ff5-4df0-9957-6d8150542dff', url: 'https://github.com/saianuragreddy/spring3-mvc-maven-xml-hello-world.git'
    }
    stage('Compile') { // Compile and do unit testing
       // run Gradle to execute compile and unit testing
       sh "mvn compile"
    }
	cleanworkspace = true
}