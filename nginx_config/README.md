### nginx 配置文件批量管理，可以更新和回滚版本.

####Author:huangxin

```
    update.yml       # 负责更新的 playbook

    backup.yml       # 控制回滚的 playbook

    new_vsion        # 更新的 角色
    
    old_vsion        # 回滚的 角色

```

> 回滚的思路：在发布新的版本之前，保存当前的版本角色的配置文件到控制回滚的角色下面，发布一次会回滚角色即可。
