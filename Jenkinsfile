pipeline{
    agent any

    stages {
  stage('build') {
    steps {
      echo 'Building .....'
    }
  }
  
  stages {
  stage('maven install') {
    steps {
      withMaven(globalMavenSettingsConfig: 'null', jdk: 'null', maven: 'null', mavenSettingsConfig: 'null') {
    sh 'mvn clean install'
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
    }
