pipeline {
      agent any
      tools {nodejs "node"}
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
       
// pipeline {
//   agent any
 
//   tools {nodejs "node"}
 
//   stages {
//     stage('Example') {
//       steps {
//         sh 'npm config ls'
//       }
//     }
//   }
// }       
       
       