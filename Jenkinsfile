pipeline {
  agent any
  stages {
    stage('Compile') {
      steps {
        echo 'CompileTest'
      }
    }
    stage('UnitTest') {
      parallel {
        stage('UnitTest') {
          steps {
            echo 'UnitTesting_Mess'
          }
        }
        stage('UiTest') {
          steps {
            echo 'TestUi'
          }
        }
      }
    }
    stage('Deploy') {
      steps {
        echo 'UiTest'
      }
    }
  }
}