pipeline{
    agent any
    

    stages{
    stage('Build Project'){
        steps{
        build 'Build'
        }
    }
    stage('Deploy to Tomcat'){
        steps{
        build 'Deploy'
        }
    }
    stage('Performance Test'){ 
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
