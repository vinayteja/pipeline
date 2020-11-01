pipeline {
 agent any
 tools {
  maven 'M2-HOME'
 }
 stages{
 stage('package') {
    steps {
    sh script: 'mvn  package'
    }
   }
 }
}
