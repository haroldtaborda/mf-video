pipeline {
    agent any
    
    tools {
        nodejs "nodejs"
    }
   stages { 
    stage('Build') {
        steps {
          sh "sudo su chmod -R 777 footer/mf-footer"
        dir('/footer/mf-footer'){
          sh "npm install"
         }
        }
    }
    
   }    
}
