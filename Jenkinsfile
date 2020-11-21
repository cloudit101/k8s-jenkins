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
                container('kubehelmjava') {
                    sh 'kubectl get pods -n jenkins'
                }
            }
        }
     }
}
 
