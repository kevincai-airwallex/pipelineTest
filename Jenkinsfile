pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''export PATH=$PATH:/usr/local/bin

npm install

'''
      }
    }
    stage('Deploy') {
      steps {
        sh '''echo "iTesting remind you:"

echo "put your deploy codes here"

echo "this is a sample example"'''
      }
    }
    stage('Test') {
      steps {
        sh '''export PATH=$PATH:/usr/local/bin

npm run smoke'''
      }
    }
  }
}