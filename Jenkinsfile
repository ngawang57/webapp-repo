pipeline {
  agent any
  stages {
    stage('compileation') {
      steps {
        build(job: 'compile', propagate: true, wait: true)
      }
    }

    stage('test') {
      steps {
        junit(allowEmptyResults: true, keepLongStdio: true, testResults: 'Hello Ngawang')
      }
    }

  }
}