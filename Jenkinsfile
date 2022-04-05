
pipeline {
  agent {label 'linux'}
  stages {
    stage('Example') {
      steps {
        sh '''
        echo "Hello world.."

        aws s3 cp index.js s3://gitlab-website001
        '''
      }
    }
  }
}
