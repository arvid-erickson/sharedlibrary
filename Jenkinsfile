#!/usr/bin/groovy
// POC for Gradle building and packaging library

node {
    // def server = Artifactory.server url: SERVER_URL, credentialsId: CREDENTIALS
    // def rtGradle = Artifactory.newGradleBuild()
    // def buildInfo = Artifactory.newBuildInfo()
    def localGradle = '/usr/local/bin/gradle'
    def buildDir = '/Users/arviderickson/.jenkins/workspace/PipelineTest/sharedLibrary'
    def repo = 'https://github.com/arvid-erickson/sharedLibrary'
    def ArtifactRepo = '/Users/arviderickson/github'
    
    stage ("Clone") {
        sh "echo Clone ${repo} to build"
        sh "git clone ${repo}"
    }

    stage ('Artifactory Config') {
          sh "echo Artifactory stuff"
          sh "echo This is not implemented yet"
          sh "echo Artifactory not available yet"
    }

    stage ('Gradle build') {
        sh "cd ${buildDir}; ${localGradle} clean build "
    }

    stage ("Publish build info") {
        // server.publishBuildInfo buildInfo
        sh "echo Publish build info"
        sh "cp ${buildDir}/build/libs/*.jar ${ArtifactRepo}"
    }
    stage ("Clean build") {
        sh "rm -rf ${buildDir}"   
    }
}
