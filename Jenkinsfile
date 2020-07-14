pipeline {
    agent any
    stages {
        stage('Upload to AWS') {
        steps {
            withAWS(region:'us-west-2',credentials:'AKIAWT4337AL2MAJH7MU') {
            s3Upload(pathStyleAccessEnabled:true, payloadSigningEnabled: true, file:'index.html', bucket:'shahzebjenkins')
          }
        }
      }
    }
}