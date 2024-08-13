# PowerOfMathCalculationt-Through-AWS

Hi friends,
   Today I host a small website in aws regarding PowerOfMathCaluclation. The folllowing services are used in aws.
   1.AWS Amplify 2.Lamda  3.IAM 4.ApiGateway 5.Dynamodb.
   
Procedure :  
1.download the attched index.html file which contains wep page code and host it on aws amplify. Copy the url and paste it on new tab. It is your web page.
2.download lambda function code file which contains code for executing math functioality and upload in your lambda function. Also you can test the code by configuring test event.
3.Go to API Gateway in aws. Create restapi and post method. Also enable cores. Then you can deploy api. Now you can copy url and paste it on index.html file so that this api gateway url is to invoke your lambada function.
4.To save the math function results, we need dynamodb table. So please create one table in AWS Dynamodb. Finally copy the arn of table.
5.We need to give access for lambda to write dynamodb table. Go to your created lambda function- click configuration - click role-click add permission and add inline policy.In that you need to attach our policy code which is attached in this repo. Please paste arn of dynamodb table in that policy code.
6.Now refresh your web page and make some math calculations.
