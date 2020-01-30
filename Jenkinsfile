pipeline {
	agent any
	stages {
		stage("Cleaning") {
			steps {
					sh "mvn clean"
			}
    	}
    	stage("Testing") {
			steps {
					sh "mvn test"
			}
    	}
		stage("Packaging") {
			steps {
					sh "mvn package"
			}
    	}
	}
}
