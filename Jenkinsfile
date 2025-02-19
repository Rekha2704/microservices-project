pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'docker build -t rekha2704/service:v1 .'
            }
        }
        stage ("push") {
            steps {
                script {
                   // This step should not normally be used in your script. Consult the inline help for details.
                     withDockerRegistry(credentialsId: 'docker-cred') {
                     // some block
                   }
                }   
            }
        }
    }
}
