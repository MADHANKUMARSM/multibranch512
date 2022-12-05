node('slave_lab') 
{
 stage('continuous download') 
{
    git 'https://github.com/sunildevops77/maven.git'
}

stage('continuous build')
{
    sh 'mvn package'
}
}
