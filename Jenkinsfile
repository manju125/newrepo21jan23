pipeline{
	agent any
	stages{
		stage("cleaning stage"){
			steps{
				sh "mvn clean"
			}
		}
		stage("Testing stage"){
			steps{
				sh "mvn test"
			}
		}
		stage("package stage"){
			steps{
				sh "mvn package"
			}
		}
		stage("Deployment stage"){
			steps{
				sh "mvn tomcat7:undeploy tomcat7:deploy"
			}
		}
	}
}
