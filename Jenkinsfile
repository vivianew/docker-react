pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo "Hello World"'
        sh '''
          echo "Multiple line also works"
          ls -lah
        '''
      }
    }
    stage('Example') {
        steps {
            echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
        }
    }
  }
}