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
        bat 'e:;cd E:\Amog java\testng;run.bat'
      }
    }
    stage('deploy') {
      steps {
        echo 'deployed'
      }
    }
  }
}
