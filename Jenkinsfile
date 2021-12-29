pipeline {
	agent any
	tools {
		jdk 'jdk11'
	}

	stages {
		stage("build") {
			steps {
				echo "building..."
			}
		}

		stage("test") {
			steps {
				echo "testing..."
			}
		}
		stage("version") {
			steps {
				sh '''
				java -version
				'''
			}
		}
	}
}