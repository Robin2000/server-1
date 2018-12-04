[![Build Status](https://travis-ci.org/elysium-project/server.svg?branch=development)](https://travis-ci.org/elysium-project/server)

# Bug reporting缺陷报告:
Before opening any bug reports on the issue tracker, please read the guidelines 在问题跟踪板块提交缺陷报告之前，请先阅读[located here](https://github.com/elysium-project/server/blob/development/docs/).

# Development process overview开发过程综述:
Any development work should be done in local feature branches rather than on the main branches used for QA/live builds. 任何开发工作应该在本地的功能分支中完成，而不是在主分支中，主分支用于问答和发布。For example, if you were working on a boss script, rather than committing directly to the development branch, you should first create a new branch with a descriptive name.例如，如果你工作内容是boss怪物的脚本，不要直接提交到开发分支，而应该创建一个新的分支，启一个新的名字。

When you have finished working on your fix or feature, you should open a pull request to allow for your code to be automatically compiled by the continuous integration system and reviewed by other developers. 当你完成了修复功能，你应该打开pull request让你的代码被持续集成系统自动编译，以及其他开发者复核。After receiving feedback and making any requested changes, your pull request will be squashed and merged to the development branch. 收到任何回馈以及变更请求，你的pull request将被压缩且合并到开发分支。Squashing your commits is to ensure that the development branch can be compiled at any point in its history as well as ensuring a clean history.压缩你的提交是为了确保开发分支可以在任何时间点编译，确保干净的修改历史。

The development branch is used as the basis for the QA and PTR realms. 开发分支被用于基本的问答和PTR领域。To ensure the QA team receives ample opportunity to test each set of changes, the development branch will only accept pull requests for one week before being frozen for a week, during which time only essential fixes will be accepted.为了确保问答团队有充足的机会测试每批变更，开发分支每周将仅接收1次pull request。然后冻结1周，期间只接收必要的修改。

Once the development branch has been tested by QA, it will be merged with the stable branch to become the next revision for the live realms. 一旦开发分支被问答团队测试通过，将合并到稳定分支成为下一个活动的修正版。The only changes accepted to the stable branch, outside of the merge window, will be critical hotfixes to resolve game-breaking and stability issues.稳定分支仅接受这样的变更，合并窗口期外，只解决游戏终端和稳定性问题的关键热修补。

As with any open source project, the workflow is subject to change as we receive feedback and discover what works best for the project and its contributors.正如任何一个开源项目，工作流程变更也会发生，当我们收到反馈且发现存在更有利项目和代码贡献者的方法时。
