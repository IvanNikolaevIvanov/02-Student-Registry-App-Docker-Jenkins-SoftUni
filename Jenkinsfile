pipeline {
 agent any
 stages {
    stage('NPM Install') {
        steps {
            bat 'npm install'
        }
        
   }
    stage('Parallel Execution') {
     parallel {
        stage('Execute Tests') {
        steps {
            bat 'npm test'
           }
        }
        stage('Execute Tests') {
        steps {
            bat 'npm test'
            }
        }
     }
    }
 }
}