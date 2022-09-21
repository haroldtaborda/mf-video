pipeline {
    agent any
    
    tools {
        nodejs "nodejs"
    }
   stages { 
    stage('Build') {
        steps {
          sh "chmod u=rw,g=r,o=r footer/mf-footer"
          sh "chmod o+rw footer/mf-footer"
        dir('/footer/mf-footer'){
          sh "npm install"
         }
        }
    }
    
   }    
}
