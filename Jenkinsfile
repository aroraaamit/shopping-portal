pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'this is the compile job'
        sh 'npm package'
      }
    }

   

    stage('package') {
      steps {
        echo 'this is the package job'
        sh 'npm run package'
      }
    }

    stage('archive') {
      steps {
        archiveArtifacts '**/distribution/*zip'
      }
    }

  }
  tools {
    nodejs 'nodejs'
  }
  post {
    always {
      echo 'this pipeline has completed...'
    }

  }
}
