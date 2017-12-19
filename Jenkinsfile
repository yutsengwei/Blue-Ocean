pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        build(job: 'black_hole_build_image', propagate: true, wait: true, quietPeriod: 5)
      }
    }
  }
}