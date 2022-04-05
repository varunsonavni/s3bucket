
pipeline {
  agent {label 'linux'}
  stages {
    stage('Example') {
      steps {
        sh '''
        echo "Hello world.."
//         aws configure set region $AWS_DEFAULT_REGION 
//         aws configure set aws_access_key_id $AWS_ACCESS_KEY_ID 
//         aws configure set aws_secret_access_key $AWS_SECRET_ACCESS_KEY
        aws s3 cp index.js s3://gitlab-website001
        '''
      }
    }
  }
}
