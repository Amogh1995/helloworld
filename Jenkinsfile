pipeline {
  agent any
  stages {
    stage('error') {
      steps {
        parallel(
          "s1": {
            echo 'This is the start'
            
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
        bat "cd /d e:\amog java\testng"
        bat "run.bat"
      }
    }
    stage('deploy') {
      steps {
        echo 'deployed'
      }
    }
  }
}
