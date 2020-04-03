pipeLine {
	agent any
	stages {
		stage ('Build') {
			steps {
				echo 'Running pipeLine'
				sh './gradlew build --no-daemon'
				archiveArtifacts artifacts: 'dist/trainSchedule.zip'
			}
		}
	}
}
