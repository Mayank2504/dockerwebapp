node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockerHub') {

        def customImage = docker.build("malacophonous/dockerwebapp:0.3")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
