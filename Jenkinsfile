pipeline {
  agent any

  tools {nodejs "node"}

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