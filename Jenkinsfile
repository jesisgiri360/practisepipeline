pipeline 
{
    agent any

    stages 
    {
        stage('build') 
        {
            steps 
            {
                echo 'building application'
            }
        }
        stage('test') 
        {
            steps 
            {
                echo 'testing application'
            }
        }
        stage('deploy') 
        {
            steps 
            {
                echo 'deploying application'
            }
        }
    }
    post 
    {
      always 
      {
        emailext body: 'summary ', subject: 'pipeline status ', to: 'jesisgiri360@gmail.com'
      }

    }
}
