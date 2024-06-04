pipeline {
    agent {
        dockerfile {
            additionalBuildArgs  '--build-arg ROS_DISTRO=humble --progress=plain '
            args '--entrypoint=\'\''
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