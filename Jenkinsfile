pipeline {
    agent any
    
    stages {
        stage('Test') {
            steps {
         
		            sh 'docker build -t test-app:v1 .'
		           
            }
        }
      stage('RUN') {
        steps {
                 sh 'docker run -d -p 80:80 test-app:v1'
       	    }
      }
    }
}
