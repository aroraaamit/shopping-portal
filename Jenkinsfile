pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'this is the compile job'
        sh 'npm install'
      }
    }

    stage('test') {
      steps {
        echo 'this is the test job'
        sh 'npm test'
      }
    }

    stage('package') {
      steps {
        echo 'this is the package job'
        sh 'npm package'
      }
    }

<<<<<<< HEAD
    stages{
        stage('build'){
            steps{
                echo 'this is the compile job'
                sh 'npm install'
                
            }
        }
        stage('test'){
            steps{
                echo 'this is the test job'
                sh 'npm test'
                
            }
        }
        stage('package'){
            steps{
                echo 'this is the package job'
               sh 'npm run  package'
               
            }
        }
=======
    stage('archive') {
      steps {
        archiveArtifacts '**/distribution/*zip'
      }
>>>>>>> 2b038ae0c6e579786611905d14d9db273b1ab432
    }

  }
  tools {
    nodejs 'nodejs'
  }
  post {
    always {
      echo 'this pipeline has completed...'
    }
<<<<<<< HEAD
    
 }
=======

  }
}
>>>>>>> 2b038ae0c6e579786611905d14d9db273b1ab432
