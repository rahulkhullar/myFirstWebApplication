node{
  stage('SCM Checkout')
  git 'https://github.com/rahulkhullar/myFirstWebApplication'
}
stage ('Compile-Package') {
  sh 'mvn package'
}

}
