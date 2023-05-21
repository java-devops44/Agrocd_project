pipeline{

    agent any

    stages{

        stage("git checkout"){

            steps{

                script{

                     git branch: 'main', credentialsId: 'gitcred', url: 'https://github.com/java-devops44/Agrocd_project.git'

                }
            }
        }

        stage("unit testing"){

            steps{

                script{

                    sh "mvn test"
                }
            }
        }

        stage("integration test"){

            steps{

                script{

                    sh "mvn verify _DskipUnitTests"
                }
            }


        }
    }
}