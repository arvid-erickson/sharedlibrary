#!/usr/bin/groovy

env.workspace = ''
if(env.BRANCH_NAME =~ /PR-\d+){retuen}
properties([[$class: 'ParametersDefinitionProperty', perameterDefinitions: [
    string(name: 'BRANCH', defaultValue: "$env.BRANCH_NAME}", description: "Name of branch to run script on"),
    [$class: 'ChoiceParameter', choiceType: 'PT_SINGLE_SELECT', description: 'Release build or single deployment?' name: 'JOB_TYPE', script: [$class: 'GroovyScript', script: [classpath: [], sandbox: true, script: `retuen ["RELEASE","DELIVERY","RESTART_INSTANCE","STAART_INSATNCE","STOP_INSTANCE"']]]
    ]
// node {
//    def server = Artifactory.server url: SERVER_URL, credentialsId: CREDENTIALS
//    def rtGradle = Artifactory.newGradleBuild()
    // def buildInfo = Artifactory.newBuildInfo()
    
    stage ('Clone') {
//        git clone 'https://...'
    }

    stage ('Artifactory Config') {
//        rtGradle.tool = "Gradle-2.4"
        // Set Artifactory repositories for dependancies resolution and artifacts deployment
//        rtGradle.deployer repo:'ext-release-local', server: server
//        rtGradle.resolver repo:'remote-repos', server: server
    }

    stage ('Gradle build') {
//        def buildInfo = rtGradle.run rootDir: "some/directory"
    }

    stage ('Publish build info') {
//        server.publishBuildInfo buildInfo
    }
// }
