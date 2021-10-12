pipeline{
    agent {label : 'MASTER'}
     triggers:{pollSCM('* * * * *')}
     stages{
         stage('clone'){
             steps{
                 git branch:'declartivepipeline',url:'https://github.com/dumrepo/spring-petclinic.git'
             }
        stage('compile'){
            steps{
               sh 'mvn package'
            }
          }
         }
     }
}
