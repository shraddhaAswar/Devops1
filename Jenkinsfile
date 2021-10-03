pipeline {
    agent any
    stages {
        stage('Building the code') {
            steps {
                echo 'Building the code'
				sh 'mvn clean install'
            }
        }
		
		
		
    }
    post { 
        always { 
            echo 'Sending email over gmail'
        }
    }
}