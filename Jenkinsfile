node('built-in') 
{
 stage('continuous download_loans') 
{
    git 'https://github.com/sunildevops77/maven.git'
}

stage('continuous build_loans') 
{
    sh 'mvn package'
}

stage('continuous deployment_loans') 
{
    sh 'scp /home/ubuntu/.jenkins/workspace/Scriptedpipeline/webapp/target/webapp.war ubuntu@172.31.13.155:/var/lib/tomcat9/webapps/qaenv.war'
}
}
