node{
  stage('SCM Checkout'){
    git 'https://github.com/hub4you365/maven-hello-app'
  }
  stage('Compile-Package'){
    def mvnHome = tool name: 'maven-3', type: 'maven'
    sh "${mvnHome}/bin/mvn clean package"
  }
}