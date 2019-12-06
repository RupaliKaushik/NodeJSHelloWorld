pipeline {
    agent any
    tools {nodejs "nodejs"}
         stages {
             stage('Checkout'){
                  steps {
                        echo "Checking out the file from Github"
                        }
             }
             stage('Build') {
                   steps {
                         echo "Creating a build"
                         sh "npm install"
                         }

                         
             }   
             stage('Test') {
                   when{
                         not{
                               branch "master"
                            }
                         }
                    steps {
                        echo "Running the Unit Tests"
                        }
              }       
             stage('Deploy') { 
                              steps {
                                    echo "Deploying the code"
                                     }
                              }
                          
                        }
                  }
       
       
       
       