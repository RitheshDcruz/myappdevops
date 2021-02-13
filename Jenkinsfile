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

			Just testing every email we sent

			Regards,
			Rithesh D\'cruz''', cc: 'ritheshdcruz30@gmail.com', from: 'ritheshdcruz30@gmail.com', replyTo: '', subject: 'Test email', to: 'ritheshdcruz30@gmail.com'
		}
		stage('Slack notification'){
			def message ="Hi from Rithesh"
			slackSend baseUrl: 'https://hooks.slack.com/services/', 
			channel: '#devops', 
			message: "${message}", 
			teamDomain: 'personal-qe42778', 
			tokenCredentialId: 'slack-demo', 
			username: 'Rithesh D cruz'
		}
		
		

	       
	
	
}