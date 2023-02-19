pipeline{
          agent any
          stages{
            stage('Build'){
                 steps{
                     sh 'g++ -c main/hello.cpp'
                     sh 'g++ -o PES1UG21CS810 main/hello.cpp'
                     echo 'Build stage successfull'
                 }
             }
             stage('Test'){
                  steps{
                      sh './PES1UG21CS810'
                      echo 'Test stage successful'
                   }
              }
             stage('Deploy'){
                  steps{

                     echo 'Deployment Successful'.
                   }
              }
           }
          post{
             failure{
                 echo 'Pipeline Failed'
              }
          }
       }
