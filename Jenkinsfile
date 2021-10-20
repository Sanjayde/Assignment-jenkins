pipeline {
    agent any
    
    stages {
        stage('Test') {
            steps {
         
		            sh 'sudo docker build -t test-app:v1 .'
		           
            }
        }
      stage('RUN') {
        steps {
                 sh 'sudo docker run -d -p 8040:80 test-app:v1'
       	    }
      }
    }
}
