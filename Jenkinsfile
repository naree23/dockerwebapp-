node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockrhub') {

        def customImage = docker.build("naree23/nodeapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
