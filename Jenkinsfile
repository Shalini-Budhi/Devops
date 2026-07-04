pipeline {
  agent any
  stages {
    stage('error') {
      steps {
        sh '''@Library(\'pipeline-library-demo\')_

 stage(\'Demo\') {
     echo \'Hello world\'
     sayHello \'Alex\'
 }'''
        build(job: 'new', quietPeriod: -1, waitForStart: true)
      }
    }

  }
}