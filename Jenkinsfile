pipeline {
  agent any
  stages {
    stage('Dev') {
      steps {
        sleep(time: 1, unit: 'MICROSECONDS')
      }
    }
    stage('Test') {
      steps {
        s3Download(file: 'index.html', bucket: 'udacity-websiteme', path: 'https://udacity-websiteme.s3.amazonaws.com/', payloadSigningEnabled: true, force: true, pathStyleAccessEnabled: true)
      }
    }
  }
}