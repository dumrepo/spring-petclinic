pipeline{
    agent {label 'MASTER'}
     triggers {pollSCM('* * * * *')}
     stages{
          stage ('clone and compile'){
             steps {
                 git branch: 'declartivepipeline', url:'https://github.com/jaligamakarthik/spring-petclinic.git'
                 sh 'mvn compile'
             }
         }
     }
}
