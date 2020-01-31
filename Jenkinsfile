pipeline {
	agent any
	stages {
		stage("Cleaning") {
			
			steps {
				sh "/opt/maven/bin/mvn clean"
			}
    		}
    		stage("Testing") {
			steps {
				sh "/opt/maven/bin/mvn test"
			}
    		}
		stage("Packaging") {
			steps {
				sh "/opt/maven/bin/mvn package"
			}
    		}
	}
}
