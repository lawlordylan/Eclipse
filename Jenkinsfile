pipeline {
    agent any
    
    stages {
        stage('Build') { 
            steps {
                sh 'mvn -f .\studenttest\pom.xml -B -DskipTests clean package' 
            }
        }
        stage('Test') { 
            steps {
                sh 'mvn -f .\studenttest\pom.xml test' 
            }
        }
    }
}
