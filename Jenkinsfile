@Library("shared-library") _

node('podman')  {
    timestamps {
        sh "whoami"
        sh "podman --version"
        sh "git --version"
        jobManager(this)
        //TagBuild(this)
        DockerBuildAndPush(this)
    }
}
