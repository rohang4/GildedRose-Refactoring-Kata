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
 stage ('---surefire-report---'){
     steps {
            sh "mvn surefire-report:report"
            }
     }		 
}
}
