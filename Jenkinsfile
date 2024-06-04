pipeline {
    agent any
    stages {
        stage('Initialize docker'){
            def dockerHome = tool 'controller-docker'
            env.PATH = "${dockerHome}/bin:${env.PATH}"
        }
        stage ("Docker build") {
            steps {
                sh("docker build --build-arg ROS_DISTRO=humble .")
            }
        }
    }
}