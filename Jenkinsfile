node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', '51fcee36-509d-4aaa-927f-fc8a1ad1e67a') {

        def customImage = docker.build("ayushgoud1502/btechproject")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
