pipeline
{
agent any
stages
{

stage("SCM Check")
{
steps
{
git branch: 'Master', url: 'https://github.com/Pankaj-git1/Cloud_Formation.git'
}
}



stage('SCM Check')
{
steps
{
sh "export AWS_DEFAULT_REGION=us-east-1"
sh "aws cloudformation create-stack --stack-name myteststack --template-body file://S3Bucket.json --region 'us-east-1'"
}
}
}
}
