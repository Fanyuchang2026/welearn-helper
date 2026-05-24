# WeLearn Helper v1.0.0

WE Learn (SFLEP) 自动刷课/刷时长工具

致敬初代版本开发者：Avenshy & SSmJaE

## 功能

- **课程刷取**：自动完成课程练习，支持指定/随机正确率
- **时长刷取**：多线程并发累积学习时长，实时进度显示
- **双模式登录**：支持账号密码登录和 Cookie 登录

## 使用方法

1. 双击 `run_welearn.bat` 运行
2. 或直接运行 `welearn.exe`

### 从源码运行

```bash
pip install requests
python welearn_decompiled.py
```

### 打包 exe

```bash
pip install pyinstaller
pyinstaller --onefile --name welearn welearn_decompiled.py
```

## 注意事项

- 本工具仅供学习交流使用
- 需要 WE Learn (SFLEP) 有效账号
- Windows 系统需开启代理以访问 welearn.sflep.com

## 更新日志

### v1.0.0 (2026-05-24)
- 适配 2026 年新 SSO 登录系统 (OIDC)
- 时长刷取改为多线程并发 + 实时进度刷新
- 课程刷取支持双重提交策略（指定正确率 + 100%正确率）
- 新增网络请求重试机制
