pipeline {
  agent any
  stages {
    stage('') {
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
        build(job: 'j1', quietPeriod: 4, wait: true)
        bat 'run.bat'
      }
    }
    stage('deploy') {
      steps {
        echo 'deployed'
      }
    }
  }
}