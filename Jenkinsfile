@Library('jenkins-library@master') _

pipeline {
    agent any
    stages {
        stage('Git Checkout') {
            steps {
            gitCheckout(
                branch: "main",
                url: "https://github.com/spring-projects/spring-petclinic.git"
            )
            }
    }
    }
}
