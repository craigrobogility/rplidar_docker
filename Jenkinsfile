pipeline {
    agent {
        dockerfile {
            additionalBuildArgs  '--build-arg ROS_DISTRO=humble --progress=plain'
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