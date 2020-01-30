pipeline {
	def mvnHome = tool 'M2_HOME'
	agent any
	stages {
		stage("Cleaning") {
			steps {
				sh "'${mvnHome}/bin/mvn' clean"
			}
    		}
    		stage("Testing") {
			steps {
				sh "'${mvnHome}/bin/mvn' test"
			}
    		}
		stage("Packaging") {
			steps {
				sh "'${mvnHome}/bin/mvn' package"
			}
    		}
	}
}
