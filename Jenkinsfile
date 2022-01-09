pipeline {
  agent {
    node {
      label 'java7'
    }

  }
  stages {
    stage('1st stage') {
      parallel {
        stage('1st stage') {
          steps {
            echo 'did 1st'
          }
        }

        stage('2nd') {
          steps {
            echo '2nd done'
          }
        }

      }
    }

  }
}