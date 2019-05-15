pipeline {
    agent {
        label 'master'
    }
	stages {
		stage('checkout') {
			steps {
				echo 'checkout'
			}
		}
		stage('Build') {
			steps {
				echo 'Build'
			}
		}
		stage('Test') {
			steps {
				echo 'test'
			}
		}
		stage('Sonar') {
			steps {
				echo 'Sonar'
			}
		}
		stage('Deployement') {
			steps {
				echo 'Deployement'
			}
		}
	}
}