pipline{
    agent{
        label "jenkins-agent"
    }
    tools{
        jdk 'Java17'
        maven 'Maven3'
    }
     stages{
       stage("Cleanup Workspace"){
            steps {
                cleanWs()
            }
        }
     }

    stages{
       stage("Checkout from SCM"){
            steps {
                 git branch: 'main', credentialsId: 'github', url: 'https://github.com/fabiog76/complete-prodcution-e2e-pipeline'
            }
        }
     }
}