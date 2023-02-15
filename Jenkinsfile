pipeline
{
  agent any
  tools
  {
		maven 'maven3.9.0'
  }
  stages{
    stage ('checkoutcode')
    {
        steps
      {
        git changelog: false, credentialsId: 'jenkins_credentials', poll: false, url: 'https://github.com/maheshgamyadevops/maven-web-application.git'        
      }
    }
	stage ('build')
    {
        steps 
      {
			sh "mvn clean package"
      }
    }
  }
  
}
