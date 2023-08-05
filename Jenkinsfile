@Library('my_shared_lib') _

pipeline{

    agent any

    stages{
         
        stage('Git Checkout'){

            steps{

                script{

                  gitCheckout(
                     branch: "main",
                     url: "https://github.com/Nageshcloud/mrdevops_java_app.git"
                    )

                }
            }
        }
        stage('maven test'){

            steps{

                script{

                  mvnTest()

                }
            }
        }
        stage('build'){

            steps{

                script{

                  mvnBuild()

                }
            }
        }
    }
}

    