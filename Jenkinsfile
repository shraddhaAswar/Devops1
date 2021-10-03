pipeline {
    agent any
    stages {
        stage('Building the code') {
            steps {
                echo 'Building the code'
				sh 'mvn clean install'
            }
        }
		
		
		stage('Testing the code') {
            steps {
                echo 'Testing the code'
				sh 'mvn test'
            }
        }
		
    }
    post { 
        always { 
            echo 'Sending email over gmail'
        }
    }
}