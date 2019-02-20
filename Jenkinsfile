pipeline {
  agent any
  stages {
    stage('Notify-Event') {
      steps {
        sh '''pipeline {
    agent none
    stages {
        stage(\'Publish Event\') {
            steps {
                publishEvent simpleEvent(\'SamanEvent\')
            }
        }
    }
}'''
        }
      }
    }
  }