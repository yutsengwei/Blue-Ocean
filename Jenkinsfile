pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            build(job: 'black_hole_build_image', propagate: true, wait: true, quietPeriod: 5)
          }
        }
        stage('gggg') {
          steps {
            echo '15615656'
          }
        }
      }
    }
    stage('send noti') {
      steps {
        emailext(subject: '123', body: 'test success', attachLog: true)
      }
    }
  }
}