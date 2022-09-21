pipeline {
    agent any
    
    tools {
        nodejs "nodejs"
    }
   stages { 
    stage('Build') {
        dir('footer/mf-footer'){
            sh 'npm install'
        }
         dir('header/mf-header'){
            sh 'npm install'
        }
    }
    
    stage('Test') {
        dir('footer/mf-footer'){
            sh 'ng test'
        }
        dir('header/mf-header'){
            sh 'ng test'
        }
    }
    
     stage('Deploy') {
        dir('footer/mf-footer'){
            sh 'npm start'
        }
        dir('header/mf-header'){
            sh 'npm start'
        }
      }
   }
}
