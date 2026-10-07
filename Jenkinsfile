pipeline{
    agent any
    stages{
        stage('checkout'){
            steps{
                deleteDir()
                sh '''
                     git clone https://github.com/bilalabdulla911-blip/nginx-deploy.git
                     ls -l
                '''
            }
        }
        stage('deploy'){
            steps{
             sh'''
                cp -r nginx-deploy/* /var/www/html
                ls -l /var/www/html
            '''
            }
        }
    }
}

            
