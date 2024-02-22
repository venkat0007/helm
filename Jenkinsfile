pipeline { 
 agent any {
 }
      stages{
       stage("cloning the url"){
       script {
           sh 'git clone https://github.com/venkat0007/helm.git -b main'
	   }
	   }
	   
	  stage ("deploying the backendapplication to k8s"){
	   script {
	     sh 'helm upgrade --install backend . --values values-devtest.yaml'
	     }
	     }
	     }
	     }
