pipeline {
	agent any


	stages {
		stage('Prep') {
			steps{
				script {
					openshift.newProject("nima-123","--display-name", "Nima 123")
					openshift.withCluster{
						openshift.withProject('nima-0123'){
						}
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
