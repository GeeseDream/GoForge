# GitHub 操作指南

此文档描述了如何与 GitHub 仓库进行交互，包括获取文件内容、更新文件内容、创建新文件和获取仓库文件列表的操作。

## 配置说明

https://raw.githubusercontent.com/GeeseDream/GPTForge/main/.instructions/instructions.md

## 仓库列表

- GTPs
  - 所有者: GeeseDream
  - 仓库名: GPTForge

## 操作说明

### 获取文件内容

操作: GetContentAtPath

- 需要信息: 仓库所有者(OWNER)，仓库名称(REPO)，文件路径(PATH)

### 更新文件内容

操作: UpdateContentAtPath

- 需要信息: 仓库所有者(OWNER)，仓库名称(REPO)，文件路径(PATH)，需要更新的文件内容(base64编码)，提交信息(message)，提交者信息(committer)

### 创建新文件

操作: CreateFileAtPath

- 需要信息: 仓库所有者(OWNER)，仓库名称(REPO)，文件路径(PATH)，新文件的内容(base64编码)，提交信息(message)，提交者信息(committer)

### 获取仓库文件列表

说明: API定义中未提供此操作，但用户可以通过指定仓库的根路径("/")来获取仓库的树形结构，从而获取文件列表。

## 操作确认

在执行任何仓库操作之前，模型都将询问用户是否确认他们的操作。这是为了确保用户了解他们的操作可能会对仓库造成的影响，并有机会在执行操作前撤销或修改他们的请求。