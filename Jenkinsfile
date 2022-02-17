pipeline {
  agent {label 'linux'}
  options {
    buildDiscarder(logRotator(numToKeepStr: '5'))
  }
  stages {
    stage('Build') {
      steps {
        echo "build"
      }
    }
    
    stage('for the x branch') {
      when {
        branch "random"
      }
      steps {
        echo "whatever branch"
      }
    }
    
    stage('fot the pr') {
      when {
        branch "PR-*"
      }
      steps {
        echo "pr"
      }
    }
    
    
  }
}
