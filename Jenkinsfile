node
{
    stage('SCM checkout')
    {
        git 'https://github.com/javahometech/my-app'
    }
    stage('MVN package')
    {
        sh 'mvn clean package'
    }
    stage('Build Docker image')
    {
        sh 'docker build -t santhosh.thoddin/my-app:2.0.0 .'
    }
}
