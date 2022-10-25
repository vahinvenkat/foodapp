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
                 
              }
          }
    }
}
