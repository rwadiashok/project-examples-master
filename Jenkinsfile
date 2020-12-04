pipeline {
  agent any
  stages {
    stage('Buzz Buzz') {
      steps {
        echo 'BeesBuzz'
      }
    }

    stage('Bees Bees') {
      steps {
        echo '"Buzz, Bees, Buzz!"'
      }
    }

    stage('\'Fluffy Deploy\'') {
      steps {
        echo 'Placeholder'
      }
    }

    stage('Buzz Test') {
      steps {
        sh './jenkins/test-all.sh'
      }
    }

    stage('artifact') {
      steps {
        archiveArtifacts(fingerprint: true, artifacts: 'target/*.jar')
      }
    }

  }
}