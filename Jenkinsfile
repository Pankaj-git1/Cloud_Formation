pipeline
{
agent any
stages
{

Stage("SCM Check")
{
stage
{
steps
{
git branch: 'Master', url: 'https://github.com/Pankaj-git1/Cloud_Formation.git'
}
}
}


stage('SCM Check')
{
steps
{
sh "export AWS_DEFAULT_REGION=us-east-1"
Sh "aws cloudformation create-stack --stack-name myteststack --template-body file://S#Bucket.json --region 'us-east-1'"
}
}
}
}
