// Powered by Infostretch 

timestamps {

node () {

	stage ('SampleAssignment - Checkout') {
 	 checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'bc4d6d6e-fbc3-4262-b73d-6a30109bc7f7', url: 'https://github.com/Nilesh108/emoji-search.git']]]) 
	}
	stage ('SampleAssignment - Post build actions') {
/*
Please note this is a direct conversion of post-build actions. 
It may not necessarily work/behave in the same way as post-build actions work.
A logic review is suggested.
*/
		// Mailer notification
		step([$class: 'Mailer', notifyEveryUnstableBuild: true, recipients: 'nilesh.mailbox1@gmail.com', sendToIndividuals: true])
 
	}
}
}