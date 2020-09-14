pipeline {
 agent any 
  stage('scm checkout') {
    git 'https://github.com/vijaykumarbandi/pipeline.git'
   }
   stage('package') {
    def mvn = tool (name : 'M2-HOME', type: 'maven') + '/bin/mvn'
    sh "${mvn} clean package"
   }
  }

    
