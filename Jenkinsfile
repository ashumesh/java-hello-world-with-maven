pipeline {
    agent any

    stages {
        stage('test')
         {
            steps 
            {
                echo 'This is testing file'
            }
        }
        stage('Build')
         {
            steps 
            {
                echo 'This is build file'
            }
        }
        stage('Deploy')
         {
            steps 
            {
                echo 'This is Deploy file'
            }
        }
    }
    post
    {
        always
        {
           emailext body: 'echo "What is the status of pipeline"', subject: 'Pipeline status', to: 'ashu12.meshram@gmail.com'
        }
    }
}
