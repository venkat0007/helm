pipeline { 
 agent any
      stages{
       stage("cloning the url"){
       steps {
       script {
           sh 'git clone https://github.com/venkat0007/helm.git -b main'
	   }
	   }
	   }
	  stage ("deploying the backendapplication to k8s"){
	  steps {
	   script {
	     sh "helm upgrade --install backend . --values values-${params.env}.yaml"
	     }
	     }
	     }
	     }
	     }
