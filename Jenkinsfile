pipeline {
  agent any
  stages {
    stage('Git Checkout') {
      steps {
        script {
          git checkout
        }

      }
    }

    stage('Build') {
      steps {
        script {
          script scripts/build.sh
        }

      }
    }

  }
  environment {
    registry = 'shanthaghverdian/cicd_pipeline_4_practical_test'
  }
}