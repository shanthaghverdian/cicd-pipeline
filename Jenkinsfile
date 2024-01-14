pipeline {
  agent any
  stages {
    stage('Git Checkou') {
      steps {
        script {
          checkout scm
          def customImage = docker.build("${registry}:${env.Build_ID}")
        }

      }
    }

  }
  environment {
    registry = 'shanthaghverdian/cicd_pipeline_4_practical_test'
  }
}