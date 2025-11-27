pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'chmod a+x run_build_script.sh'
        sh './run_build_script.sh'  
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
