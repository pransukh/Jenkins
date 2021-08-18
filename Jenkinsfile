pipeline{
 agent any
 stages{
    stage('Compile Stage'){
       steps{
              withMaven(maven : 'Maven_3.8.2')
              {
              sh 'mvn clean compile'
             }
       }
    }

    stage('Test Stage'){
           steps{
                  withMaven(maven : 'Maven_3.8.2')
                  {
                  sh 'mvn test'
                 }
           }
        }
        stage('Deploy Stage'){
               steps{
                      withMaven(maven : 'Maven_3.8.2')
                      {
                      sh 'mvn deploy'
                     }
               }
            }
 }
}