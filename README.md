# 女巫的毒药 GitHub Pages 版

这个文件夹可以直接上传到 GitHub 仓库，用 GitHub Pages 发布。

## 文件说明

- `index.html`
  游戏主页面
- `words.json`
  词库配置文件。以后只需要改这个文件，不需要改网页代码。

## 词库格式

`words.json` 必须保持下面这个结构：

```json
{
  "title": "女巫的毒药",
  "rounds": [
    {
      "name": "第1轮",
      "words": [
        { "en": "English", "zh": "中文" }
      ]
    }
  ]
}
```

注意：

- 每一轮必须正好有 `9` 个单词。
- 每个词条都要同时有 `en` 和 `zh`。
- 可以增加轮数，不一定只能 2 轮。

## GitHub Pages 发布步骤

1. 注册或登录 GitHub。
2. 新建一个公开仓库，例如 `witch-poison-game`。
3. 把这个文件夹中的 `index.html` 和 `words.json` 上传到仓库根目录。
4. 进入仓库 `Settings`。
5. 打开 `Pages`。
6. 在 `Build and deployment` 中选择：
   - `Source`: `Deploy from a branch`
   - `Branch`: `main`
   - `Folder`: `/ (root)`
7. 保存后等待 GitHub Pages 部署完成。
8. 公开网址通常会是：
   `https://你的GitHub用户名.github.io/仓库名/`

## 后续替换单词

以后只要：

1. 修改 `words.json`
2. 提交并推送到 GitHub

网页内容就会自动更新，学生继续访问同一个链接即可。
