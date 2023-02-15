pipeline
{
  agen any
  stages{
    stage ("checkoutcode")
    {
        steps
      {
        git changelog: false, credentialsId: 'jenkins_credentials', poll: false, url: 'https://github.com/maheshgamyadevops/maven-web-application.git'        
      }
    }
  }
  
}
