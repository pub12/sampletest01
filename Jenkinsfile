pipeline {
	agent any 
	stages {
		stage('build') {
			steps {
				sh 'docker version'
			}
		}

		stage ('sanity check'){
			steps{
				input "move to prod?"
			}
		}

		stage ('prod'){
			sh 'python --version'
		}
	}
}
