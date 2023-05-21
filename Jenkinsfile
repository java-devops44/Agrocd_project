pipeline{

    agent any

    environment{

        DOCKER_USERNAME = "cloudhub12"
        APP_NAME = "gitops-agro-app"
        IMAGE_TAG = "${BUILD_NUMBER}"
        IMAGE_NAME = "${DOCKER_USERNAME}" + "/" + "${APP_NAME}"
        REGISTORY_CRID = "dockerhub"

    }
    stages{

        stage('checkout the code'){

            steps{

                script{

                    git branch: 'main', credentialsId: 'gitcred', url: 'https://github.com/java-devops44/Agrocd_project.git'
                

            }
        }
    }
}

   