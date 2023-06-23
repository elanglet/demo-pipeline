pipeline {
  agent any
  stages {
    stage('Récupération du code') {
      steps {
        git(url: 'https://github.com/elanglet/projet-banque', branch: 'master')
      }
    }

    stage('Maven') {
      steps {
        bat 'mvn install'
      }
    }

  }
}