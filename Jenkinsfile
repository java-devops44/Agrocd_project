pipeline {
    
    agent any 
    
    stages {
        
        stage('Git Checkout'){
            
            steps{
                
                script{
                    
                    git branch: 'main', credentialsId: 'gitcred', url: 'https://github.com/java-devops44/Agrocd_project.git'
            }
        }

        stage('UNIT testing'){

            steps{

                script{

                    sh 'mvn test'
                }
            }
        }
    }
}

   