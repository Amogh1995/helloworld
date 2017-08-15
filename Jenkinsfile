pipeline {
  agent any
  stages {
    stage('error') {
      steps {
        parallel(
          "s1": {
            echo 'This is the start of hygieia'
            
          },
          "sub s1": {
            echo 'this  is sub'
            
          }
        )
      }
    }
    stage('r1') {
      steps {
        echo 'fdsdf'
      bat '''cd /d e:/amog java/testng
run
'''
        
      }
    }
    stage('deploy') {
      steps {
        echo 'deployed'
      }
    }
  }
}
