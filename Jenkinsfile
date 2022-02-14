pipeline {
	agent any
	tools {
		jdk 'jdk11'
		gradle 'gradle6'
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