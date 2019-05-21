pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            sh '''sleep 60

export PATH=$PATH:/usr/local/bin

npm install

'''
          }
        }
        stage('SequenceRunAfterBuild') {
          steps {
            sh '''

echo "run after build, not parallel run"


'''
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