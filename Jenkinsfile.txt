node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', '1530dacb-f1b7-4bea-bf81-dc909ef1744d') {

        def customImage = docker.build("ayushgoud1502/btechproject")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
