pipeline {
  agent any
  stages {
    stage("build") {
      steps {
        sh """
          docker build -t hello_there ./docker-test
        """
      }
    }
    stage("run") {
      steps {
        sh """
          docker run --rm hello_there
        """
      }
    }
  }
}
