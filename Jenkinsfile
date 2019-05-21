pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            sh '''export PATH=$PATH:/usr/local/bin

npm install

'''
          }
        }
        stage('SequenceRunAfterBuild') {
          steps {
            sh '''echo "run after build, not parallel run"

sleep 60

echo "1 minute sleep"'''
          }
        }
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