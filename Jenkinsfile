pipeline {
	agent any
	stages {
		stage('Prep') {
			steps{
				echo "$env.openshift-project"
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
