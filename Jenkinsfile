pipeline {
    agent any
    stages {
        stage ("Docker build") {
            steps {
                sh("docker buildx create --name builder --bootstrap --use || echo 'already exists'")
                sh("docker buildx build --platform linux/arm64,linux/amd64 --progress=plain --build-arg ROS_DISTRO=humble .")
            }
        }
    }
}