pipeline {
  agent any
  stages {
    stage('Say Hello') {
      steps {
        echo 'Hello world!'
      }
    }

    stage('Build') {
      steps {
        sh 'docker build -t appsbymatthew .'
      }
    }

    stage('Run') {
      steps {
        sh 'docker run --publish 5000:5000 appsbymatthew'
      }
    }

  }
}