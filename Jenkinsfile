node('master')
{
    stage ('continuousdownload-test')
    {
        git 'https://github.com/selenium-saikrishna/maven1.git'
    }
    stage ('continuousbuild-test')
    {
        sh 'mvn package'
    }
    stage ('continuousdeployment-test')
    {
        sh 'scp /home/ubuntu/.jenkins/workspace/multibranch_test/webapp/target/webapp.war ubuntu@172.31.14.183:/var/lib/tomcat7/webapps/qeen.war'
    }
}
  
  
  
  
  
  
  
  

