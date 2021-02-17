node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockerhub') {
        def customImage = docker.build("ork44/webapplication")
        /* Push the container to the custom Registry */
        customImage.push()
    }
}