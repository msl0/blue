pipeline {
  agent {
    node {
      label 'node'
    }

  }
  stages {
    stage('cmd') {
      steps {
        sh 'hostname'
      }
    }

    stage('linux') {
      parallel {
        stage('build') {
          steps {
            echo 'build'
          }
        }

        stage('windows') {
          steps {
            echo 'build'
          }
        }

      }
    }

    stage('archive') {
      steps {
        echo 'archive'
      }
    }

  }
}