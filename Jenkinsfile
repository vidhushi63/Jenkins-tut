pipeline {
  agent any
  environment {
      name = "abc"

  }
  stages{
    stage ('test1'){
      agent any
      steps {
        sh '''
        date
        ls
        pwd
        '''
      }
      stage ('Environment variable'){
          sh '''
          echo ${name}
          echo ${BUILD_ID}
          '''
   
      }
}
