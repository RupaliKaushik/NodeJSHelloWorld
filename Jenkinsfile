pipeline{
    agent any
         stages{
             stage('One'){
                  steps{
                        echo "Hi,This is Rupali"
                        }
             }
             stage('Two'){
                   steps{
                         input('Do you want to procees?')
                         }
             }   
             stage('Three'){
                   when{
                         not{
                               branch "master"
                            }
                         }
                    steps{
                        echo "Hello"
                        }
              }       
             stage('Four'){
                     parallel{
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
       
                                      
                                      
    
    
    
