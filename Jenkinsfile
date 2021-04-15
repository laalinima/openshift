pipeline {
	agent any
	stages {
		stage('Prep') {
			steps{
				sh "oc policy add-role-to-user edit system:serviceaccount:cicd:default -n ${params.openshift_project}"
				sh "oc project ${params.openshift_project}"
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
