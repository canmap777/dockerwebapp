node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'mmcanada') {

        def customImage = docker.build("mmcanada/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
