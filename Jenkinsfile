node {
def mvn = tool (name: 'M2-HOME', type: 'maven') + '/bin/mvn'
stage('SCM Checkout'){
git 'https://github.com/vijaykumarbandi/pipeline.git'
}
 stage('Mvn Package'){
  sh "${mvn} clean package"
   }
}
