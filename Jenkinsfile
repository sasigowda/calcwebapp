pipeline{
    stage('Build Project'){
        build 'Build'
    }
    stage('Compile Package'){
        build 'Deploy'

    }
    stage('Deploy to Tomcat'){ 
        build 'PerformTest'
    }
    stage ('Deploy to Artifactory"){
        build 'test-artifactory'
    }
}
