pipeline {
  agent any
  stages {    
    stage('Cloning Git') {
      steps {
        git 'https://github.com/pankajwebay/node_jenkin_app.git'
      }
    }        
    stage('Install dependencies') {
      steps {
        sh 'npm i -save express'
      }
    }     
    stage('Test') {
      steps {
         sh 'node app.js'
      }
    }             
  }
}