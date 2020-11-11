

pipeline {
    agent any
    triggers {
    pollSCM('* * * * *')
  }

    environment {
        default_branch = 'master'
    }
    stages {
        stage('Git Checkout') {
            steps {
checkout([$class: 'GitSCM',
          branches: [[name: '*/master']],
          userRemoteConfigs: [[url: 'https://github.com/sindhams/quickstart-microsoft-sql.git']]
          changelog: false,
          poll: false
])
            }
    }
    }
}

