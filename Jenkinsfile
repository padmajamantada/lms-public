pipeline {
    agent any
    stages 
{
        stage('gIT checkout') 
      {
            steps {

               git branch: 'main', url: 'https://github.com/padmajamantada/lms-public.git'
          }

        }
        stage('Docker-build') {
            steps {
                sh 'docker build -f /lms-public/Dockerfile' 
            }
   }
}
