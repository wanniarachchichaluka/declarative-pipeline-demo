pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        bat 'run_build_script.bat'  
      }
    }
    stage('Test') {
      parallel {
        stage ('Test on Windows') {
          steps {
            echo "Running tests on Windows"
          }
        }
        stage ('Test on Linux') {
          steps {
            echo "Running tests on Linux"
          }
        }
      }
    }
  }
}
