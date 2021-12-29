pipeline {
	agent any
	tools {
		jdk 'jdk8'
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