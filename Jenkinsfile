pipeline {
agent {
docker {
image 'maven:latest' // Use the Maven Docker image as the build environment
}
}
stages {
    stage('Build and Test') {
        steps {
            script {
                // Clone the repository and build the Java application
                git '<https://github.com/callSyedOsman/2048>'
                sh 'mvn clean install' // Assuming Maven is used for building the Java application
            }
        }
    }
