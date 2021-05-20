#!/usr/bin/groovy
// POC for Gradle building and packaging library

node
{
    stage('Checkout')
    {
        GitManager.clone(this, "https://github.com/jfrogdev/project-examples.git", "*/master", "myGitUserID");
    }
}
