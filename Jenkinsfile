pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        build(job: '${service}', quietPeriod: -2)
      }
    }
  }
}