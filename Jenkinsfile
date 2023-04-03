pipeline {
    agent any 
    stages {
        stage("Build") {
            steps {
                sh "mvn clean -f ansible"
            }
        }
        stage ('Test') {
            steps {
                sh "mvn test -f ansible"
            }
        }
        stage ("Deploy") {
            steps {
                sh "mvn package -f ansible"
            }
        }
    }
}
