1. create namespace

kubectl create namespace tektontutorial &&\
kubectl config set-context --current --namespace=tektontutorial


第一部分： Pipeline Resources
目的：
理解 pipeline Resource 的功能和作用
创建 pipeline Resource

1. 前提条件：
确认环境 Kubernetes 版本 v1.19+
kubectl version --short
看到如下的输出：
Client Version: v1.20.0
Server Version: v1.20.0

确认 Tekton piplines 已经部署，并且 API 可用：
kubectl api-resources --api-group='tekton.dev'
看到如下输出：
NAME                SHORTNAMES   APIGROUP     NAMESPACED   KIND
clustertasks                     tekton.dev   false        ClusterTask
conditions                       tekton.dev   true         Condition
pipelineresources                tekton.dev   true         PipelineResource
pipelineruns        pr,prs       tekton.dev   true         PipelineRun
pipelines                        tekton.dev   true         Pipeline
runs                             tekton.dev   true         Run
taskruns            tr,trs       tekton.dev   true         TaskRun
tasks                            tekton.dev   true         Task

2. 创建 Create a pipeline resource




3. 
