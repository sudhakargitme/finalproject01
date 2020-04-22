node {
    checkout scm

    docker.withRegistry('https://hub.docker.com/', 'dockerhub') {

        def customImage = docker.build("firstshipment/npmimg02")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
