pipeline 
{
    agent any

    stages 
    {
        stage('Build') 
        {
            steps 
            {
                echo 'Application building'
            }
        }
        stage("Testing")
        {
            steps
            {
                echo 'Running the application in testing phase'
            }
        }
        stage("Deploy")
        {
            steps
            {
                echo 'Running the application in deployment '
            }
        }
    }
    
    post
    {
        always
        {
            emailext body: 'Summery', subject: 'pipeline status', to: 'shubhamguptaid73@gmail.com'
        }
    }
}
