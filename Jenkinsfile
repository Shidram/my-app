node{
  stage('SCM Checkout'){
  git 'https://github.com/Shidram/my-app'
  }
  stage('Compile-Package'){
    // Get the Maven home path
    def mvnHome = tool name: 'maven-3', type: 'maven'
    sh "${mvnHome}/bin/mvn package"
  }
  stage("Email Notification"){
    mail bcc: '', body: '''Hi Welcome to jenkins email alert.

Thanks
Shidramshetti''', cc: '', from: '', replyTo: '', subject: 'Jenkins Job Successfully Completed', to: 'shidramshetty@gmail.com'
  }
}
