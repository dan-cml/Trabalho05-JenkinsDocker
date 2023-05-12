pipeline {
  agent { label "linux" }
  stages {
    stage("build") {
      steps {
        sh """
          docker build -t ola-unicamp .
        """
      }
    }
    stage("run") {
      steps {
        sh """
          docker run --rm ola-unicamp
        """
      }
    }
  }
}
