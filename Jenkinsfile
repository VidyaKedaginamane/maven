pipeline {
    agent any
    stages {
        stage('Example') {
           steps { bat "exit 0" }
        }
    }
    post { 
	failure {
	   mail body: 'Hi Vidya', subject: 'The Pipeline failed', to: 'scmlearningcentre@gmail.com'
        }
    }
}
