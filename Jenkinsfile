node{
  stage('SCM checkout'){
  git credentialsId: 'gitID', url: 'https://github.com/arpan13579/docker-app'
  }
  stage('Compile Package'){
  def mvnHome = tool name: 'maven3', type: 'maven'
  sh "${mvnHome}/bin/mvn package"
  }

}
