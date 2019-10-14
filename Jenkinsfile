pipeline {
    agent { docker { image 'python:3.7' } }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
				sh 'pip install pytest'
            }
        }
		stage('test') {
			steps {
				sh 'pytest -v'
			}
		}
    }
}
