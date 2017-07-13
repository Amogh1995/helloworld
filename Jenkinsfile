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
        bat "e:"
        bat "cd Amog java
        bat "cd testng"
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
