node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'saptapdiz') {

        def customImage = docker.build("saptapadiz/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
