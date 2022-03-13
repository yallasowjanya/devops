pipeline 
{
    agent any

    stages 
    {
        stage('Build') 
        {
            steps
            {
                echo 'Build App'
            }
        }
        
        stage('Test') 
        {
            steps
            {
                echo 'Test App'
            }
        }
        
        stage('Deploy') 
        {
            steps
            {
                echo 'Deploy App'
            }
        }
        
        stage('email') 
        {
            steps
            {
               emailext body: 'summary', recipientProviders: [buildUser()], subject: 'pipeline', to: '3b8sowjanya@gmail.com' 
            }
        }
    }
}
