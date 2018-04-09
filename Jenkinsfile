pipeline {

	agent any
	
	stages {
	   
		stage('build'){
	          steps {
		    
			sh 'cd /var/lib/jenkins && java -jar jenkins-cli.jar -s http://172.31.118.70:8080/ -auth admin:haminepal1 get-job "git_integration_test" > job.xml && java -jar jenkins-cli.jar -s http://localhost:8080/ -auth admin:haminepal1 create-job "git_integration_test" < job.xml'	

}
}

}

}
