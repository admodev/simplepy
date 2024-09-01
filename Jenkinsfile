pipeline {
	agent docker {
		image: 'python:3.9-slim'
		args: '-v /var/jenkins_home:/var/jenkins_home'
	}
	stages {
		stage('Setup') {
			steps {
				sh 'echo "Python version is:"'
				sh 'python --version'
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
