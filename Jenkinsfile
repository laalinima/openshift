pipeline {
	agent any
	stages {
		stage('Prep') {
			steps{
				echo "${params.openshift_project} World!"
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
