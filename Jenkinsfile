pipeline
{
    agent {node {label 'mikryus'}}

    stages
    {
        stage('test')
        {
            steps{
                echo "test30"
            }
        }
        stage('newgrp docker')
        {
            steps{
                sh 'newgrp docker'
                sh 'whoami'
            }
        }
        stage('build docker')
        {
            steps{
                sh 'docker build -t obraz_nginx:1.0 .'
            }
        }

        stage('run docker')
        {   
            steps{
                sh 'docker run -d -it -p 8080:80 --name nginx_app obraz_nginx:1.0'
            }
        }
    }
}