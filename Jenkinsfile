@Library('my-shared-library') _

pipeline{
    agent any

    stages{
        stage('Git Checkout'){
            steps{
                script{
                    gitCheckout(
                        branch: "main",
                        url: "https://github.com/DevTiti/java-app.git"
                    )
                }
            }
        }

        stage('Unit Test maven'){
            steps{
               script{
                  mvnTest()
               }
             }
        }
    }
}