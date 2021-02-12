pipeline {
	agent {
	    label 'linux-slave'  
	}
	stages{
	    stage('scm checkout '){
			steps{
 				echo "slveeeeeeeeeeeeeeeeeeee"
				git 'https://github.com/RitheshDcruz/myappdevops.git'
			}
			stage('Compile package')
			{
				steps{
					def maven_home=tool name: 'maven-3', type: 'maven'
					sh "${mvnHome}/bin/mvn package"

				}
			}
	       
	    }
		
        
	}
	


}