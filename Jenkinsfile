pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        bat 'chmod a+x run_build_script.sh'
        bat './run_build_script.sh'
      }
    }
    stage('Test') {
      steps {
       echo "Run tests" 
      }
    }
  }
}
