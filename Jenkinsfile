pipeline{
    agent any
         stages{
             stage('One'){
                  steps{
                        echo "Checking out from git"
                        }
             }
             stage('Two'){
                  steps{
                         echo "Creating a build"
                        }
                        
             }   
            stage('Three'){
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
       
             stage('Four'){
                   steps{
                         input('Do you want to proceed?')
                         }
                          }   
             stage('Five'){
                    steps{
                        echo "Deploy"
                        }
                          }       
             
       }
       }
}
       
                                      
                                      
    
    
    
