#!/usr/bin/groovy

node {
//    def server = Artifactory.server url: SERVER_URL, credentialsId: CREDENTIALS
//    def rtGradle = Artifactory.newGradleBuild()
    // def buildInfo = Artifactory.newBuildInfo()
//    def localGradle = '/usr/local/bin/gradle'
    def localGradle = 'which gradle'
    
    stage ("Clone") {
//        git clone 'https://...'
//        sh "echo Clone repo to build"
    }

    stage ('Artifactory Config') {
//        rtGradle.tool = "Gradle-2.4"
        // Set Artifactory repositories for dependancies resolution and artifacts deployment
//        rtGradle.deployer repo:'ext-release-local', server: server
//        rtGradle.resolver repo:'remote-repos', server: server
//        sh "echo Artifactory stuff"
//        sh "echo This is not implemented yet"
//        sh "echo Artifactory not available yet"
    }

    stage ('Gradle build') {
//        def buildInfo = rtGradle.run rootDir: "some/directory"
        sh "cd /Users/arviderickson/.jenkins/workspace/P*1/sharedLibrary"
        sh "which gradle"
        sh "${localGradle} build"
    }

    stage ("Publish build info") {
//        server.publishBuildInfo buildInfo
//        sh "echo Publish build info"
//        sh "./gradle clean build"
    }
    stage ("Clean build") {
          sh "rm -rf /Users/arviderickson/.jenkins/workspace/"   
    }
}
