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
        s3DoesObjectExist(bucket: 'udacity-websiteme', path: 'index.html')
      }
    }
  }
}