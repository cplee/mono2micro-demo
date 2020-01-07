# Setup
* Reset namespace
  * `helm --tiller-namespace reinvent19-staging delete --purge springtrader`
  * `git push origin skaffold:master`
  * wait for codepipeline to complete...
  * `git push origin 9f6b24d:master --force`
  * `git push origin skaffold:skaffold`
  * Create <a href="https://console.aws.amazon.com/codesuite/codecommit/repositories/springtrader/pull-requests/new/master/.../refs/heads/skaffold?region=us-east-1" target="_blank">PR</a>
  * `kubectl config use-context microk8s`
* Open <a href="https://console.aws.amazon.com/codesuite/codepipeline/pipelines/springtrader/view?region=us-east-1" target="_blank">CodePipeline</a>
* Open <a href="https://springtrader.reinvent19-staging.lead.prod.liatr.io/spring-nanotrader-web" target="_blank">app</a>
* Open <a href="https://istio-system.lead.prod.liatr.io/kiali/console/graph/namespaces/?edges=requestsPerSecond&graphType=versionedApp&namespaces=reinvent19-staging&unusedNodes=false&injectServiceNodes=true&duration=60&pi=15000&layout=dagre" target="_blank">kiali</a>
