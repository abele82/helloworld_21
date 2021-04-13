pipeline {
    agent any
  tools {
    maven 'M2_HOME'
  }

    stages {
        stage('Build') {
            steps {
                sh 'mvn clean'
                sh 'mvn install'
                sh 'mvn package'
                
            }
        }
         stage('Test') {
            steps {
                echo 'Hello test'
                sleep 5
            }
        }
         stage('Deploy') {
            steps {
                echo 'Hello Deploy'
                sh 'pwd'
            }
        }
                stage('push') {
            steps {
                echo 'Hello push'
                sh 'dockerps'
              
            }
        }
    }
}  
