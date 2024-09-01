pipeline {
	agent any
	stages {
		stage('Setup') {
			steps {
				sh 'echo "Python version is:"'
				sh 'python3 --version'
			}
		}
		stage('Run') {
			steps {
				sh 'pwd'
				sh 'python3 .'
				sh 'echo "Finished!"'
			}
		}
	}
}
