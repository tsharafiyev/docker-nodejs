node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockerhub') {

        def customImage = docker.build("timur1988/nodejs-app")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
