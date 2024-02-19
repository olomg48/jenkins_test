pipeline
{
    agent {node {label 'mikryus'}}

    stages
    {
        stage('test')
        {
            steps{
                echo "siematest21112"
            }
        }

        stage('build docker')
        {
            steps{
                sh 'docker build -t obraz_nginx:1.0'
            }
        }

        stage('run docker')
        {   
            steps{
                sh 'docker run -p 80:80 --name nginx_app obraz_nginx:1.0'
            }
        }

        /*stage("sprzatanie")
        {
            steps{
                sh 'cd /home/jenkins'
                sh 'rm -r jenkins_test'
            }
        }*/
    }
}