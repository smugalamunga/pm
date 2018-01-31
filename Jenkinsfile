node('maven') {
  checkout scm
  stage('Build') {
    sh "mvn -s configuration/settings.xml install"
    stash name: "war", includes: "target/pm*.war"
  }
}
