node {
    checkout scm

    docker.withRegistry('https://hub.docker.com/repository/docker/ork44/test', 'dockerhub') {

        def customImage = docker.build("test/dockerwebapp")
        def docker = "my docker"
        /* Push the container to the custom Registry */
        customImage.push()
    }
}