pipeline{
    agent any
    

    stages{
    stage('Build Project'){
        steps{
        build 'Build'
        }
    }
    stage('Compile Package'){
        steps{
        build 'Deploy'
        }
    }
    stage('Deploy to Tomcat'){ 
        steps{
        build 'PerformTest'
        }
    }
    stage ('Deploy to Artifactory'){
        steps{
        build 'test-artifactory'
        }
    }
    }
}
