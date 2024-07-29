pipeline {
  agent any
  stages {
    stage('Fetch Code ') {
      steps {
        git(url: 'https://github.com/jagdeepR/BlueOrepo.git', branch: 'main')
      }
    }

    stage('Install Apache') {
      steps {
        sh 'sudo apt install apache2 -y'
      }
    }

    stage('deploying application') {
      steps {
        sh 'sudo cp -R * /var/www/html/'
      }
    }

  }
}