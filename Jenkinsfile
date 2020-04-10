pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'mvn install'
      }
    }

    stage('Unit Test') {
      steps {
        sh 'mvn test'
      }
    }

    stage('Deployement') {
      steps {
        sh 'mvn spring-boot:run'
        sh 'sh exit 0'
      }
    }

  }
  tools {
    maven 'M3'
  }
}