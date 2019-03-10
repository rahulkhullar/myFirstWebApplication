node{
  stage('SCM Checkout') {
  git 'https://github.com/rahulkhullar/myFirstWebApplication'
}
stage ('Compile-Package') {
  sh 'mvn package'
  // get maven home path
  //def mvnHome = tool name: 'maven-3', type: 'maven'
  
}

}
