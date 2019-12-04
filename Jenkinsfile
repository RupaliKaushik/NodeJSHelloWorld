pipeline {
    agent any
    stages {
        stage('One') {
            steps {
                echo "Checking out from git"
            }
        }
        stage('Two') {
            steps {
                echo "Creating a build"
            }

        }
        stage('Three') {
           
                
                    steps {
                        echo "Running the Unit Test"
                    }
                
                
                
            

            stage('Four') {
                steps {
                    input('Do you want to proceed?')
                }
            }
            stage('Five') {
                steps {
                    echo "Deploy"
                }
            }

        }
    }
}