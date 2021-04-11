github action 工作流结构
```
- workflow
  - workflow file: .github/workflows 下的 yaml 配置文件
    - job: 多个可以顺序或并行执行，它下面的所有 step 都在一个 runner 内执行，多个 step 可以共享信息
      - step
        - 命令
        - action: 工作流的最小单元，可以自己创建，也可以使用 action 商店开源的
  - event: 触发工作流的事件，如 push 到仓库
  - Runner: 安装了 github action runner 应用程序的机器，它每次只允许一个 job
  - Artifact: 工作流产出的文件
```