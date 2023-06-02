pipeline {
  agent any
  stages {
    stage('Stage 1') {
      steps {
        echo 'Step 1'
      }
    }

    stage('Stage 2.1') {
      parallel {
        stage('Stage 2.1') {
          steps {
            sh 'echo \'Step 2.1\''
          }
        }

        stage('Stage 2.2') {
          steps {
            sh 'echo \'Step 2.2\''
          }
        }

      }
    }

  }
}