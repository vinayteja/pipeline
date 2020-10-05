pipeline {
 agent any
 tools {
  maven 'M2-HOME'
 }
 stages{
 stage('scm checkout') {
    git 'https://github.com/vijaykumarbandi/pipeline.git'
   }
   stage('package') {
    steps {
    sh script: mvn 'clean package'
    }
   }
 }
}
