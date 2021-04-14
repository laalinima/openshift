pipeline {
	agent any


	stages {
		stage('Prep') {
			steps{
				script {					
					openshift.withCluster{
						sh "oc policy add-role-to-user edit system:serviceaccount:cicd:jenkins -n $env.openshift-project"
						openshift.withProject("nima-123"){
							sh 'oc version'
							sh 'oc project nima-123'
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
