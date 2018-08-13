node{
  stage('SCM Checkout'){
    git 'https://github.com/hub4you365/maven-hello-app'
  }
  stage('Compile-Package'){
    def mvnHome = tool name: 'maven-3', type: 'maven'
    sh "${mvnHome}/bin/mvn package"
  }
  stage('Email Notification'){
    mail bcc: '', body: '''ようこそJenkins Emailアラート
 ありがとうございます。
 以上です。''', cc: '', from: '', replyTo: '', subject: 'Jenkins Job', to: 'hub4you365@gmail.com'
  }
}