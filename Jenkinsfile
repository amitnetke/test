pipeline {
    agent {
        label 'master'
    }
	stages {
		stage('checkout') {
			steps {
				echo 'checkout..'
			}
		}
		stage('Build') {
			expression {
				return env.BRANCH_NAME != 't';
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