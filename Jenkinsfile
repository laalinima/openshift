pipeline {
	agent any


	stages {
		stage('Prep') {
			steps{
				script {					
					openshift.withCluster{						
						openshift.withProject("nima-123"){
							sh "oc get all -o wide"
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
