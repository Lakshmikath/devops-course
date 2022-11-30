pipeline {
    agent any
    parameters {
	choice(name: 'VERSION', choices: ['1.1.0','1.2.0','1.3.0'], description:'')
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
            echo "deploying version ${VERESION}"
            '''
        }
    }
 }
}
