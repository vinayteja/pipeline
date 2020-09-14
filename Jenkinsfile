pipeline {
agent any
 stages {
stage('git checkout') {
git 'https://github.com/vijaykumarbandi/pipeline.git'
}
stage('compile-package') {
def mvnHome = tool name: 'M2-HOME', type: 'maven'
 sh "${mvnHome}/bin/mvn package"
}
}
}

