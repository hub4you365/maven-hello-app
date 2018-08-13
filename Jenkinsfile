node{
  stage('SCM Checkout'){
    git 'https://github.com/hub4you365/maven-hello-app'
  }
  stage('Compile-Package'){
    tool name: 'maven-3', type: 'maven'
    sh 'mvn package'
  }
}