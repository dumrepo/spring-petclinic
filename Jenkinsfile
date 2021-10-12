pipeline{
    agent {label 'MASTER'}
    trigger {pollSCM('* * * * * ')}
        stages{
                stage{
                    steps('clone and compile')
                    branch : 'declartivepipeline',
                    url:'https://github.com/jaligamakarthik/spring-petclinic.git'
                    sh 'mvn compile'
                }
        }
}
