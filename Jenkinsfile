pipeline {
	agent {
		docker { image 'node:7-alpine' }
	}
	stages {
		stage('Test') {
			steps {
				sh 'node --version'
			}
		}
	}
	
	stage('Build') {
		steps {
			echo 'Building...'
			echo "Running ${env.BUILD_ID} ${env.BUILD_DISPLAY_NAME} on ${env.NODE_NAME} and JOB ${env.JOB_NAME}"
		}
	}
	stage('Test') {
		steps {
			echo 'Testing...'
		}
	}
	stage('Deploy') {
		steps {
			echo 'Deploying...'
		}
	}
	
}
