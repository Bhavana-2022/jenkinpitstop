pipeline {
    agent{
        label 'bhavana'
    }
    triggers{
        pollSCM('* * * * *')
    }
    stages{
        stage('vcs'){
           steps{
               git url: 'https://github.com/Bhavana-2022/jenkinpitstop.git',
                   branch: 'main'

        
           }
        }
        stage('build') {
            steps{
                sh 'dotnet build pipeline/src/pitstop.sln'
            }


        }
    
    }
}    

