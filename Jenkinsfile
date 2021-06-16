pipeline {
    agent {
        node {
        label 'LinuxGeneric'
        }
    }
    options {
        disableConcurrentBuilds()
    }
    environment {
        consultool = "gonsul"
    }

    stages {
        stage('Check Tools') {
            steps {
                sh "make -v"
                sh "go version"
            }}
        
        stage('Compile') {          
            steps {
                sh "make build"
            }
            
        }

        stage('Test') {
            steps {
                echo 'Real test...'
                // build job: 'cloud-operational-configuration/development', quietPeriod: 0
            }}


    }
    
}

