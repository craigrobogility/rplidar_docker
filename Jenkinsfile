pipeline {
    agent any
    stages {
        stage ("Docker build") {
            steps {
                sh("docker build --build-arg ROS_DISTRO=humble .")
            }
        }
    }
}