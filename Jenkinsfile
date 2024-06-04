pipeline {
    agent {
        dockerfile {
            label 'built_by_jenkins'
            additionalBuildArgs  '-build-arg ROS_DISTRO=humble'
        }
    }
}