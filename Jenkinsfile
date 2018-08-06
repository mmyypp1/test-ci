node('master') {
	stage('Preparation') {
		git 'https://github.com/mmyypp1/test-ci.git'
	}
	stage('Build') {
		withMaven(maven: 'Maven-3.5.2') {
			sh 'mvn -Dmaven.test.failure.ignore clean install' 
		}
	} 
}