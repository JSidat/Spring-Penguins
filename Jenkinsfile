pipeline {
    agent any
    stages {
        stage('Build') {
          steps {
                sh "mvn clean package"
            }
        }
        stage('Test') {
            steps {
                sh "java -jar target/spring-penguins-0.0.1-SNAPSHOT.jar"
            }
        }
    }
}
