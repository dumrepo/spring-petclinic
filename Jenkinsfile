pipeline{
    agent {label 'MASTER'}
     triggers {pollSCM('* * * * *')}
     stages {
          stage {
             steps {
                 git branch :'declartivepipeline', url:'https://github.com/jaligamakarthik/spring-petclinic.git'
                 sh 'mvn compile'
             }
         }
     }
}
