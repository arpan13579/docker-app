node{
  stage('SCM checkout'){
  git credentialsId: 'gitID', url: 'https://github.com/arpan13579/docker-app'
  }
  stage('Compile Package'){
  def mvnHome = tool name: 'maven3', type: 'maven'
  sh "${mvnHome}/bin/mvn package"
  }
  stage('Email Notification'){
  mail bcc: '', body: '''Hi
  Welcome to Jenkins email alert.
  Thanks
  Arpan Gupta''', cc: '', from: '', replyTo: '', subject: '', to: 'arpan6284@gmail.com'
  }

}
