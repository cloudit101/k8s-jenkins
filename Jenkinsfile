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
                container('busybox') {
                    sh 'hostname'
                }
            }
        }
     }
}
 
