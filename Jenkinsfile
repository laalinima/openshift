pipeline {
	agent any


	stages {
		stage('Setup') {
			steps{
				openshift.withProject('nima-123')								
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
