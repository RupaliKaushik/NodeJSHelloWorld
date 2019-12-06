pipeline {
    agent any
         stages {
             stage('Checkout'){
                  steps {
                        echo "Checking out the file from Github"
                        }
             }
             stage('Build') {
                   steps {
                         input('Creating a build')
                         }
                         sh 'npm run build'
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
       
       
       
       