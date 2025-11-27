pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        bat 'run_build_script.bat'  
      }
    }
    stage('Test') {
      steps {
       echo "Run tests" 
      }
    }
  }
}
