pipeline {
   
    agent {
        kubernetes {
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
 
