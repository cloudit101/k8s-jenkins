pipeline {
   
    agent {
        kubernetes {
          defaultContainer 'jnlp'
          
            
        }
    }
    stages {
        stage('Build') {
            steps {
                container('jnlp') {
                    sh 'java -version'
                }
            }
        }
     }
}
 
