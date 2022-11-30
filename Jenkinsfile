pipeline {
    agent any
  triggers {
    pollSCM '*/5 * * * *'
  }  
  stages {
      stage('Build') {
          steps{
              echo "Building.."
              sh '''
              echo "doing build stuff.."
              '''
          }
      }
      stage('Test') {
        steps{
            echo "Testing...."
            sh '''
            echo "doing test stuff.."
            '''
        }
      }
     stage('Deloyment') {
        steps {
            echo "Deployment goes here.."
            sh '''
            echo "Deploying applications"
            '''
        }
    }
 }
}
