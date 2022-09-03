pipeline {
  agent any
  stages {
    stage("build") {
      steps {
        bat 'docker build -t hello_there .'
      }
    }
    stage("run") {
      steps {
        bat 'docker run --rm hello_there'
      }
    }
  }
}
