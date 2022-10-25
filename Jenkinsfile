pipeline {
    agent 
    {
        node
        {
            label 'deployment'
        }
    }
    stages {
        
        stage('Docker install')
          {
              steps
              {
                  sh 'chmod +x Dockerinstall'
                  sh './Dockerinstall'
                 
              }
          }
        stage('docker build and deploy')
        {
            steps{
                sh 'sudo docker build . -t hotel:project'
                sh 'sudo run --name hotelproject -d -p 8085:80 hotel:project'
            }
        }    
    }
}
