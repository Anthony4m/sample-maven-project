pipeline{
    agent any

    stages {
    stage('build') {
      steps {
        echo 'Building .....'
      }
    }
    stage('maven install') {
      steps {
        withMaven() {
      bat 'mvn clean install'
        }
      }
    }
    stage('test') {
      steps {
        echo 'Testing .....'
      }
    }
    stage('deploy') {
      steps {
        echo 'Deploying .....'
        echo 'Done .....'
      }
    }
  }
}
    
