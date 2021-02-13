node {
	
	
	    stage('scm checkout'){
			
 			echo "slveeeeeeeeeeeeeeeeeeee"
			git 'https://github.com/RitheshDcruz/myappdevops.git'
			
		}
		stage('Compile package'){
			def maven_home = tool name: 'maven-3', type: 'maven'
			sh "${mvnHome}/bin/mvn package"
		}
	       
	
	
}