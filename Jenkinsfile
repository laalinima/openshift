pipeline {
	agent any


	stages {
		stage('Compile') {
			steps{
				sh "oc version"
				sh "oc project cicd"
				sh "oc get all -o wide"
			}
		}
	}
 }
