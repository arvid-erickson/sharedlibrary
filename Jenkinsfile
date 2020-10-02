#!/usr/bin/groovy


// node {
//    def server = Artifactory.server url: SERVER_URL, credentialsId: CREDENTIALS
//    def rtGradle = Artifactory.newGradleBuild()
    // def buildInfo = Artifactory.newBuildInfo()
    
    stage ("Clone") {
//        git clone 'https://...'
        sh "echo Clone repo to build"
    }

    stage ('Artifactory Config') {
//        rtGradle.tool = "Gradle-2.4"
        // Set Artifactory repositories for dependancies resolution and artifacts deployment
//        rtGradle.deployer repo:'ext-release-local', server: server
//        rtGradle.resolver repo:'remote-repos', server: server
        sh "echo Artifactory stuff"
        sh "echo This is not implemented yet"
        sh "echo Artifactory not available yet"
    }

    stage ('Gradle build') {
//        def buildInfo = rtGradle.run rootDir: "some/directory"
          sh "echo gradle clean build"
    }

    stage ("Publish build info") {
//        server.publishBuildInfo buildInfo
        sh "echo Publish build info"
//        sh "./gradle clean build"
    }
// }
