* Check status of <a href="https://console.aws.amazon.com/codesuite/codepipeline/pipelines/springtrader/view?region=us-east-1" target="_blank">CodePipeline</a>
* Create a <a href="https://console.aws.amazon.com/codesuite/codecommit/repositories/springtrader/pull-requests/3/changes?region=us-east-1" target="_blank">skaffold.yaml</a>
* Confirm new execution of <a href="https://console.aws.amazon.com/codesuite/codepipeline/pipelines/springtrader/view?region=us-east-1" target="_blank">CodePipeline</a>
* Review CodePipeline creation via CDK
![](https://d2908q01vomqb2.cloudfront.net/0716d9708d321ffb6a00818614779e779925365c/2018/08/28/CDKCompilesCFN-1-1024x265.png)
  *  <a href="https://github.com/cplee/skaffold-pipeline-cdk/blob/master/lib/skaffold-pipeline-cdk-stack.ts" target="_blank">cplee/skafffold-pipeline-cdk</a>
  *  `npm install -g aws-cdk`
  *  `cdk diff -c name=springtrader`
  *  `cdk deploy -c name=springtrader`
* TODO: eks from cloud9
  * `k -n reinvent19-staging get po`
  * `k -n reinvent19-staging get vs`
* <a href="https://springtrader.reinvent19-staging.lead.prod.liatr.io/spring-nanotrader-web" target="_blank">Try it!</a>
