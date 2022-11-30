pipeline {
  agent {
    dockerfile {
      filename 'Dockerfile'
    }

  }
  stages {
    stage('git') {
      steps {
        git(url: 'https://github.com/Ronaldosoaresdeb/jsoncrack.com.git', branch: 'main')
      }
    }

  }
}