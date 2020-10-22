#!/usr/bin/groovy

node {
//    def server = Artifactory.server url: SERVER_URL, credentialsId: CREDENTIALS
//    def rtGradle = Artifactory.newGradleBuild()
    // def buildInfo = Artifactory.newBuildInfo()
    def localGradle = '/usr/local/bin/gradle'
    def buildDir = '/Users/arviderickson/.jenkins/workspace/PipelineTest/sharedLibrary'
    def repo = 'https://github.com/arvid-erickson/sharedLibrary'
    
    stage ("Clone") {
        sh "echo Clone ${repo} to build"
        sh "git clone ${repo}"
//        
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
        sh "cd ${buildDir}; ${localGradle} clean build "
//.     sh "which gradle"
//        sh "${localGradle} build"
    }

//    stage ("Publish build info") {
//        server.publishBuildInfo buildInfo
//        sh "echo Publish build info"
//        sh "./gradle clean build"
//    }
//    stage ("Clean build") {
//          sh "rm -rf ${buildDir}/sharedlibrary"   
//    }
}
