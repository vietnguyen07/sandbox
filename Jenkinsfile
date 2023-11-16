pipeline {
  agent any
  stages {
    stage('build_env') {
      parallel {
        stage('build_env') {
          steps {
            git(url: 'https://github.com/vietnguyen07/sandbox', branch: 'master')
            echo 'pass test'
          }
        }

        stage('print msg') {
          steps {
            echo 'stage 2'
          }
        }

      }
    }

  }
}