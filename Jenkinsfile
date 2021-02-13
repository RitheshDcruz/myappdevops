node {
	
	
	    stage('Git checkout'){
			
 			echo "slveeeeeeeeeeeeeeeeeeee"
			git 'https://github.com/RitheshDcruz/myappdevops.git'
			
		}
		stage('Compile package'){
			def maven_home = tool name: 'maven-3', type: 'maven'
			sh "${maven_home}/bin/mvn package"
		}
		stage('Email notification'){
			mail bcc: 'ritheshdcruz30@gmail.com', body: '''Hi,

			Just testing every email we get

			Regards,
			Rithesh D\'cruz''', cc: 'ritheshdcruz30@gmail.com', from: 'ritheshdcruz30@gmail.com', replyTo: '', subject: 'Test email', to: 'ritheshdcruz30@gmail.com'
		}
		

	       
	
	
}