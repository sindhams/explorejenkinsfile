@Library('jenkins-library@master') _

pipeline {
    agent any
    environment {
        default_branch = 'wavefront'
    }
    stages {
        stage('Git Checkout') {
            steps {
            gitCheckout(
                branch: "${default_branch}",
                url: "https://github.com/spring-projects/spring-petclinic.git"
            )
            }
    }
    }
}
