node("master)
     {
       stage("ContinuousDownload")
       {
         git 'https://github.com/selenium-saikrishna/maven.git'
       }
       stage("ContinuousBuild")
       {
         sh 'mvn package'
       }
     }
     
