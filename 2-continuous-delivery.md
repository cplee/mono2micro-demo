* Check status of <a href="https://console.aws.amazon.com/codesuite/codepipeline/pipelines/springtrader/view?region=us-east-1" target="_blank">CodePipeline</a>
* Create a <a href="https://console.aws.amazon.com/codesuite/codecommit/repositories/springtrader/pull-requests/3/changes?region=us-east-1" target="_blank">skaffold.yaml</a>
* Confirm new execution of <a href="https://console.aws.amazon.com/codesuite/codepipeline/pipelines/springtrader/view?region=us-east-1" target="_blank">CodePipeline</a>
* Review CodePipeline creation via CDK
![](https://d2908q01vomqb2.cloudfront.net/0716d9708d321ffb6a00818614779e779925365c/2018/08/28/CDKCompilesCFN-1-1024x265.png)
  *  <a href="https://github.com/cplee/skaffold-pipeline-cdk/blob/master/lib/skaffold-pipeline-cdk-stack.ts" target="_blank">cplee/skafffold-pipeline-cdk</a>
  *  `npm install -g aws-cdk`
  *  `cdk diff -c name=springtrader`
  *  `cdk deploy -c name=springtrader`
  *   Review <a href="https://console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacks/resources?filteringText=&filteringStatus=active&viewNested=true&hideStacks=false&stackId=arn%3Aaws%3Acloudformation%3Aus-east-1%3A489130170427%3Astack%2Fspringtrader%2F99fbb780-109a-11ea-a2a8-0e0494eb61ff" target="_blank">CloudFormation</a>
* Review EKS resources
  * `aws eks update-kubeconfig --name lead`
  * `k -n reinvent19-staging get po`
  * `k -n reinvent19-staging get vs`
* <a href="https://springtrader.reinvent19-staging.lead.prod.liatr.io/spring-nanotrader-web" target="_blank">Try it!</a>
