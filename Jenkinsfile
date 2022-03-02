pipeline{
  agent {label 'francisco'}
  stages{
    stage ('Build'){
      steps{
        sh'''
        echo "inicia build"
        mvn clean install
        '''
        
        
      }
    }
    stage ('test'){
      steps{
        echo "do something"
      }
    }
    stage ('Deploy'){
      steps{
        echo "haciendo despliegue"
        sh'''
        docker cp /root/workspace/Francisco_academia/tuberia_prueba/target/sparkjava-hello-world-1.0.war tomcat://usr/local/tomcat/webapps
        '''
      }
    }
  }
}
