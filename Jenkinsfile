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
                    sh 'pwd && ls -al'
                    sh 'kubectl get nodes'                   
                    sh 'kubectl get pods -n jenkins'
                    sh 'helm list -A'
                }
            }
        }
     }
}
 
