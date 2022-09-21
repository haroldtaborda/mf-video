pipeline {
    agent any
    
    tools {
        nodejs "nodejs"
    }
   stages { 
    stage('Build') {
        steps {
        dir('/footer/mf-footer'){
          sh "npm install"
         }
        }
    }
    
   }    
}
