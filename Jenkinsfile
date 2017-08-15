node('permanent-slave') {
  stage('Code pull') {
    git credentialsId: '', url: 'https://github.com/qinyujia/Java-web-demo.git'
  }
  stage('mvn test') {
    sh 'mvn test'
  }
  stage('mvn build') {
    sh 'ls'
    sh 'mvn -Dmaven.test.skip=true package'
  }
}
