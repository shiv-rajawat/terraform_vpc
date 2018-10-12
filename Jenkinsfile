pipeline {
  agent any

  stages {

    stage('Checkout') {
        steps {
          checkout scm
        }
    }

    stage('IAM Creation'){
      steps{
        sh 'terraform init'
        sh 'terraform apply -input=false -auto-approve'
        
      }
    }

      }
}
