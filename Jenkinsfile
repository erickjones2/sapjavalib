pipeline {
	agent any
	def mvnHome = tool 'M2_HOME'
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
