pipeline {
    agent 
    {
        node
        {
            label 'deployment'
        }
    }
    stages {
        
        stage('apache2 install')
          {
              steps
              {
                  sh 'sudo apt install apache2 -y'
                  sh 'sudo rm -rf /var/www/html/*'
                  sh 'sudo cp -r  /home/ubuntu/workspace/masterproject/* /var/www/html/'
              }
          }
    }
}
