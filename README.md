# 2026-of-life-instruction
Describe my life and reflections in 2026 for review and summary.

### 2026/02/22
- 这是一个git-github-jupyterlab的实践，目标是git和github和jupyterlab之间的互通
- 提交失败，不知道为啥
- 改为ssh模式链接模式，成功的提交了。
#### 总结过程
 - 下载jupyterlab-git：用conda下载没有下载成功，改用pip下载。
 - 提交修改：用https提交没有成功，原因不详。改用ssh提交成功。
 - ssh提交流程：
 - - ls ~\.ssh\id_*   # 列出 .ssh 目录下的密钥文件
   - ssh-keygen -t ed25519 -C "your_email@example.com" #生成新的ssh
   - cat ~\.ssh\id_ed25519.pub # 查看公匙
   - 登录 GitHub，点击右上角头像 → Settings → SSH and GPG keys → New SSH key
   - ssh -T git@github.com  # 查看连接
   - git remote set-url origin git@github.com:Resendipity/2026-of-life-instruction.git # 修改本地仓库远程地址为ssh
   - git remote -v # 查看修改结果
   - origin  git@github.com:Resendipity/2026-of-life-instruction.git (fetch)
   - origin  git@github.com:Resendipity/2026-of-life-instruction.git (push) # 应显示内容
   - cd D:\file\github\2026-of-life-instruction # 修改为所在文件地址
   - git push # 再次推送
#### 用github的桌面版连接github
 - 模式和jupyterlab-git大差不差
 - 编辑器选择pycharm。模式和其他的python项目大差不差
 - 一个repository就是一个project



