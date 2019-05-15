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
			when{
				 expression {
					return env.BRANCH_NAME != 'master';
				}
			}
			steps {
				echo 'Build'
			}
		}
		stage('Test') {
			when{
				expression {
					return env.BRANCH_NAME != 'master';
				}
			}
			steps {
				echo 'test'
			}
		}
		stage('Sonar') {
			when{
				branch 'test*'
			}
			steps {
				echo 'Sonar'
			}
		}
		stage('Deployement') {
			when{
				expression {
					return (env.BRANCH_NAME == 'master' || 'dev');
				}
			}
			steps {
				echo 'Deployement'
			}
		}
	}
}