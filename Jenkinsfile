pipeline {
  agent {
    node {
      label 'linux_agents'
    }

  }
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

        stage('gcc_version') {
          steps {
            sh 'gcc -v'
          }
        }

      }
    }

  }
}