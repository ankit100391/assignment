pipeline {
    agent any
    stages {
		stage('BUILD') {
			steps {
				sh 'sleep 5'
			}
		}
        stage('TEST MULTIPLE') {
            parallel {
				stage('WINDOWS TEST') {
					steps {
                     	sh 'sleep 5'
					}
				}
				stage('LINUX TEST') {
					steps {
						sh "sleep 5"
					}
				}
            }
        }

		stage('DEPLOY') {
			parallel {
				stage('SERVER1') {
					steps {
                     	sh 'sleep 5'
					}
				}
				stage('SERVER2') {
					steps {
						sh "sleep 5"
					}
				}
            }
		}
    }
}
