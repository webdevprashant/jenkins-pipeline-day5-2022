pipeline   {

agent any 
/* agent {label 'slavecli1'} */

stages 	{
	stage('SCM')  {
		steps   	{
			echo "git pull my code step 1"
			/ * git 'https://github.com/vimallinuxworld13/simple-java-maven-app.git' */
			}
   		}
	stage('Build')  {
		steps  		{
			sh 'mvn clean package'
			}
   		}
	stage('Deploy')   {
		steps  		{
			echo "java -jar target/*.jar"
			}
   		}
	stage('Deploy to production')   {
		steps  		{
			echo "Final app in production environment"
			}
   		}
}
}