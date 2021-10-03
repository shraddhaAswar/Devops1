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
		
		stage('Deploying the code') {
            steps {
                echo 'Code has been deployed'
            }
        }
		
    }
    post { 
        always { 
            echo 'Sending email over gmail'
        }
    }
}