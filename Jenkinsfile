pipeline {
    agent any
    environment{
        PATH="/opt/apache-maven-3.9.0/bin:$PATH"
    }

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('scm') {
            steps {
               git 'https://github.com/123prema/hello-world.git'
            }  
        }
        stage('mvn') {
            steps {
               sh "mvn package"
            }  
        }
    }
}
