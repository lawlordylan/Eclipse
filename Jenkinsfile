pipeline {
    agent any
    
    stages {
        stage('Build') { 
            steps {
                bat 'mvn -f ./studenttest/pom.xml -B -DskipTests clean package' 
            }
        }
        stage('Test') { 
            steps {
                bat 'mvn -f ./studenttest/pom.xml test' 
            }
        }
    }
}
