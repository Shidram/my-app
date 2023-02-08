node{
  stage('SCM Checkout'){
  git 'https://github.com/Shidram/my-app'
  }
  stage('Compile-Package'){
    sh 'mvn package'
  }
}
