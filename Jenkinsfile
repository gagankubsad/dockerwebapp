node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'DockerHub-perso') {

        def customImage = docker.build("kubsadgagan/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
