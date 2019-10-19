pipeline {
  agent {
    docker {
      image 'ruby'
    }

  }
  stages {
    stage('build') {
      steps {
        sh 'ruby --version'
        sh 'echo "Hello, World."'
      }
    }
    stage('Test') {
      steps {
        echo 'This is only a test!'
        timeout(time: 30) {
          echo 'Quick'
        }

      }
    }
  }
}