pipeline {
	agent any
	tools {
		jdk 'jdk8'
		gradle 'gradle4'
	}

	stages {
		stage("build") {
			steps {
				echo "building..."
				sh '''
					gradle build
				'''
			}
		}

		stage("test") {
			steps {
				echo "testing..."
				sh '''
				gradle test
				'''
			}
		}
		stage("version") {
			steps {
				sh '''
				java -version				
				'''
				sh '''
				gradle -version
				'''
			}
		}
	}
}