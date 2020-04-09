node("master")
     {
       stage("ContinuousDownload")
       {
         git 'https://github.com/selenium-saikrishna/maven.git'
       }
       stage("ContinuousBuild")
       {
         sh 'mvn package'
       }
       stage("ContinuousDeployment")
          {
               sh 'scp /home/ubuntu/.jenkins/workspace/simplescript/webapp/target/webapp.war ubuntu@172.31.47.37:/var/lib/tomcat8/webapps/qaenv5.war'
          }
     }
     
