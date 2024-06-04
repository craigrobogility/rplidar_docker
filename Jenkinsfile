pipeline {
    agent {
        dockerfile {
            additionalBuildArgs  '-build-arg ROS_DISTRO=humble'
        }
    }
    stages {
        stage ('nothing') {
            steps {
                sh 'ls -l'
            }
        }
    }
}