pipeline {
    agent {
        label 'master'
    }
	stages {
		stage('checkout') {
			when{
				branch 'master'
			}
			steps {
				echo 'checkout'
			}
		}
		stage('Build') {
			when{
				branch 'master'
			}
			steps {
				echo 'Build'
			}
		}
		stage('Test') {
			when{
				branch 'master'
			}
			steps {
				echo 'test'
			}
		}
		stage('Sonar') {
			when{
				branch 'master'
			}
			steps {
				echo 'Sonar'
			}
		}
		stage('Deployement') {
			when{
				branch 'dev'
			}
			steps {
				echo 'Deployement'
			}
		}
	}
}