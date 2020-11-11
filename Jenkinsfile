@Library('jenkins-library@master') _

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
            gitCheckout(
                branch: "${default_branch}",
                url: "https://github.com/sindhams/quickstart-microsoft-sql.git"
            )
            }
    }
    }
}

