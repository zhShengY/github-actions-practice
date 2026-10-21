# github-actions-practice

开源软件设计与开发 实验二 实践项目一：使用 GitHub Actions 实现 Python 项目的自动化测试。

## 项目结构

```
.github/workflows/ci.yml   工作流配置
calculator.py              被测代码
test_calculator.py         单元测试
requirements.txt           依赖清单
```

## 工作流说明

推送代码或发起 Pull Request 时触发，在 ubuntu-latest 运行器上依次执行：检出代码、安装 Python 3.11、安装 pytest、运行 `pytest -v`。
