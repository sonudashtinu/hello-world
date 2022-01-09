pipeline {
  agent any
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

    stage('test') {
      steps {
        echo 'testing 1st'
      }
    }

    stage('Confirm Deploy to Staging') {
      steps {
        input(message: 'deploy', ok: 'do it')
      }
    }

  }
}