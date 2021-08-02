pipeline{
    agent none
    stages{
        stage("Build"){
            steps{
                echo "Build Package"
		sh 'ifconfig'
            }
        }
        stage("Test"){
            steps{
                echo "Test Package"
            }
        }
        stage("Deploy"){
            steps{
                echo "Deploy Package"
            }
        }
    }
}
