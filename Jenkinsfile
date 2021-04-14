pipeline {
	agent any


	stages {
		stage('Prep') {
			steps{
				script {					
					openshift.withCluster{
						openshift.newProject("nima-123","--display-name", "Nima 123")
					}																					
				}
			}
		}
		
		//stage('Compile') {
		//	steps{
		//		sh "oc version"
		//		sh "oc project cicd"
		//		sh "oc get all -o wide"
		//	}
		//}
	}
 }
