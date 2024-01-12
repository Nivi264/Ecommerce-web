pipeline {
        agent build-agent
    
        stages {
            stage('Checkout') {
                steps {
                    checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: '78dcd195-4800-4bfa-828b-e9613c3ab286', url: 'https://github.com/Nivi264/Ecommerce-web.git']])
                }
            }
            stage('mvn package'){
                steps{
                    bat "mvn package"
                }
            }
        }
    }

