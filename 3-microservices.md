* Copy a single service into a <a href="https://github.com/cplee/springtrader-marketsummary" target="_blank">new repo</a>
* Create Istio <a href="https://github.com/cplee/springtrader-marketsummary/pull/1/commits" target="_blank">Virtual Service</a>
* Define a new <a href="https://console.aws.amazon.com/codesuite/codepipeline/pipelines/springtrader-marketsummary/view?region=us-east-1" target="_blank">CodePipeline</a>
  *  `cdk deploy -c name=springtrader-marketsummary`
* View <a href="https://istio-system.lead.prod.liatr.io/kiali/console/graph/namespaces/?edges=requestsPerSecond&graphType=versionedApp&namespaces=reinvent19-staging&unusedNodes=false&injectServiceNodes=true&duration=60&pi=15000&layout=dagre" target="_blank">Kiali</a>
![](https://ignitelab.liatr.io/img/strangler.gif#shadow#80)
