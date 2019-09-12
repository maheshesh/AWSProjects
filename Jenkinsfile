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
        s3Download(file: 'index.html', bucket: 'udacity-websiteme', path: 'index.html', payloadSigningEnabled: true, force: true, pathStyleAccessEnabled: true)
      }
    }
  }
}