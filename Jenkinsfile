pipeline {
   
    agent {
        kubernetes {
          defaultContainer 'jnlp'
          yamlFile 'build.yaml'
            
        }
    }
    stages {
        stage('Build') {
            steps {
                container('jen') {
                    sh 'java -version'
                }
            }
        }
     }
}
 
