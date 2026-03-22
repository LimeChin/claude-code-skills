# Claude Code Skills

个人 Claude Code Skill 集合。

## 安装

### Windows

```bash
# 克隆仓库
git clone https://github.com/你的用户名/claude-code-skills.git

# 复制 skills 到用户目录
xcopy claude-code-skills\skills\*.md C:\Users\你的用户名\.claude\skills\ /Y
```

### 配置数据库

```bash
# 复制模板
copy templates\db-config.local.yml.template D:\winchannel\db-config.local.yml

# 编辑配置，填入真实数据库连接信息
```

## Skills

### analyze-requirement

分析需求文档，自动扫描代码库和数据库，生成实现方案。

**用法：**
```bash
/analyze-requirement <需求文档路径> [代码记录路径]
```

**示例：**
```bash
/analyze-requirement D:\winchannel\xuqiuwendang\vinda-nacos-dev\2026-0175.md D:\winchannel\xuqiuwendang\vinda-nacos-dev\2026-0175\经销宝下单-购物车.md
```

**功能：**
- 读取需求文档和代码记录
- 扫描代码库，找出相关文件
- 查询数据库表结构
- 分析依赖关系
- 生成实现方案供选择

## 目录结构

```
claude-code-skills/
├── skills/                          # Skill 文件
│   └── analyze-requirement.md
├── templates/                       # 配置模板
│   └── db-config.local.yml.template
└── README.md
```