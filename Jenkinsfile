agent any {
 def mvn = tool (name : 'M2-HOME', type: 'maven') + '/bin/mvn'
 stage('scm checkout') {
    git 'https://github.com/vijaykumarbandi/pipeline.git'
   }
   stage('package') {
    sh "${mvn} clean package"
   }
  }

    
