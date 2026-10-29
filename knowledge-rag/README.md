# Knowledge RAG 学习项目

从 Java 基础和资料管理小程序开始，逐步实现技术资料检索与问答系统。

项目工作目录：`D:\Projects\knowledge-rag`。

今天先打开 [2026-10-29 学习任务](notes/2026-10-29.md)，按顺序完成。Java 与 javac 已在本机命令行检查可用；在 IDEA 中选择已安装的 JDK 即可。

## 当前目录

```text
knowledge-rag/
├─ backend-learning/
│  └─ src/                 # 今天在这里编写 Java 练习
├─ notes/
│  └─ 2026-10-29.md        # 当日任务与复盘
├─ .gitignore
└─ .gitattributes
```

## 第一天任务

自行编写 `backend-learning/src/Document.java` 和 `DocumentManager.java`。

`Document` 包含 id、title、content、createdAt。资料管理器使用 ArrayList，实现新增、按 ID 查询、标题搜索、删除和打印列表。测试空值、重复 ID 和不存在的资料。今天优先完成增删查与调试，equals/hashCode 留到下一次集合练习深入。

先把控制台程序写通，再引入 Spring Boot 和数据库。

## 日常 Git 操作

在项目目录打开终端，执行：

```bash
git status
git diff
git add backend-learning/src notes
git diff --cached
git commit -m "feat: implement in-memory document manager"
git log --oneline -5
```

先查看改动，再添加并提交实际完成的内容。示例提交信息用于完成对应功能后。

## 配置文件

账号密钥放在被忽略的 `.env` 或本地配置文件中。可提交不含密钥的 `.env.example`，记录需要的变量名。
