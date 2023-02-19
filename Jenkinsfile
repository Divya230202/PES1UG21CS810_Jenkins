pipeline{
          agent any
          stages{
            stage('Build'){
                 steps{

                     echo 'Build stage successfull'
                 }
             }
             stage('Test'){
                  steps{
                      sh './PES1UG21CS810'
                      echo 'Test stage successful'
                   }
             }}}
              }
             stage('Deploy'){
                  steps{

                     echo 'Deployment Successful'
                   }
              }
           }
}mnjjb
          post{
             failure{
                 echo 'Pipeline Failed'
              }
          }
       }
