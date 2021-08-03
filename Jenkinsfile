pipeline{
    agent{
        label 'sshAgent'
    }
    stages{
        stage("Package Creation"){
            steps{
                git branch: 'master' ,
                    url: 'https://github.com/govi230/simple-java-maven-app.git'
                maven: 'maven-3.8.1'
                artifactoryMavenBuild goals: 'package'
            }
        }
    }
}
