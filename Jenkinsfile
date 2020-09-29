node {
 def mvn = tool (name : 'M2-HOME', type: 'maven') + '/bin/mvn'
 tools {
  maven 'M2-HOME'
 }
 stage('scm checkout') {
    git 'https://github.com/vijaykumarbandi/pipeline.git'
   }
   stage('package') {
    steps {
    sh script: mvn 'clean package'
    }
   }
  stage('email notification') {
   steps {
    mail bcc: '', body: '''hi 
its successful''', cc: '', from: '', replyTo: '', subject: 'Jenkins test file', to: 'vijaykumarbandi6594@gmail.com'
   }
  }
}

    
