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
             stage('Parallel') {
                     parallel {
                          stage('Unit Test') {
                                               steps {
                                                        echo "Running the Unit Test"
                                                      }
                                              }
                          stage('Integration Test') { 
                                                  
                                                steps {
                                                        echo "Running the Integration Test"
                                                      }

                                        }
                                      }
       }
       }
       }
       }