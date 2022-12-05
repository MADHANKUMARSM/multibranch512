node('build-in') 
{
 stage('continuous download') 
{
    git 'https://github.com/sunildevops77/maven.git'
}

stage('continuous build')
{
    sh 'mvn package'
}

stage('continuous deployment')
{
    sh 'scp /home/ubuntu/.jenkins/workspace/Scriptedpipeline/webapp/target/webapp.war ubuntu@172.31.13.155:/var/lib/tomcat9/webapps/qaenv.war'
}
}
