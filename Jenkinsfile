pipeline{
agent any
stages {
   stage ('---clean---'){
     steps {
            sh "mvn clean"
            }
     }			
  stage ('---test---'){
     steps {
            sh "mvn test"
            }
     }	
  stage ('---package---'){
     steps {
            sh "mvn package"
            }
     }	
  stage ('---site---'){
     steps {
            sh "mvn site"
            }
     }	
stage ('Email Notification'){
	 steps {
	 mail bcc: '', body: ''' Welcome to email alert.
	 Thanks
	 Rohan''', cc: '', replyTo: '', subject: 'Jenkins Job', to: 'gonsalvez01@gmail.com'
	 }
	 }
   
}
}
