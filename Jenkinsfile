pipeline {
    agent any
    stages {
        stage ("Docker build") {
            steps {
                sh("docker buildx build --platform linux/arm64 --build-arg ROS_DISTRO=humble .")
            }
        }
    }
}