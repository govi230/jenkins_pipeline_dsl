pipeline{
    agent{
        label 'sshAgent'
    }
    stages{
        stage("Package Creation"){
            steps{
                git branch: 'master' ,
                    url: 'https://github.com/govi230/simple-java-maven-app.git'
                withMaven(
                    maven: 'maven-3.8.1',
                    publisherStrategy: 'EXPLICIT',
                    traceability: true,
                    options: [
                        artifactsPublisher(disabled: false),
                        junitPublisher(disabled: false,ignoreAttachments: true)
                    ]){
                    sh 'mvn package'
                }
            }
        }
    }
}
