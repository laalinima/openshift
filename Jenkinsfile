pipeline {
	agent any
	stages {
		stage('Prep') {
			steps{				
				//sh "oc project ${params.openshift_project}"
				script {
                			openshift.withCluster() {
                    			openshift.withProject('${params.openshift_project}') {
                        		echo "Using project: ${openshift.project()}"
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
