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

        stage('clone repo')
        {
            steps{
                sh 'cd /home/jenkins'
                sh 'git clone https://github.com/olomg48/jenkins_test'
            }
        }

        /*stage("sprzatanie")
        {
            steps{
                sh 'cd /home/jenkins'
                sh 'rmd -r jenkins_test'
            }
        }*/
    }
}