#!/usr/bin/env groovy
pipeline {
  agent any
  environment {
    NODE_ENV_PATH = './venv'
    NODE_VERSION = '6.11.1'
  }
  stages {
    stage('Pre-cleanup') {
      steps {
   echo "preclean up done"
      }
    }
    stage('Make venv') {
      steps {
        echo " Make venv done"
      }
    }
    stage('Install dependencies') {
      steps {
        echo "Install dependencies done"
      }
    }
    stage('Run tests') {
      steps {
        echo "Run tests done"
      }
    }
  }
  post {
    failure {
      echo 'Processing failed'
    }
    success {
      echo 'Processing succeeded'
    }
  }
}