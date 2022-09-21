pipeline {
    agent any
    
    tools {
        nodejs "nodejs"
    }
   stages { 
    stage('Build') {
        steps {
          sh "chmod -R a+rw footer/mf-footer"
        dir('/footer/mf-footer'){
          sh "npm install"
         }
        }
    }
    
   }    
}
