# 头像设置说明

## 请将头像文件放在这里

请将 `lzp.jpg` 文件放在本目录（`assets/img/`）下。

## 头像要求

- **文件名**：`lzp.jpg`（必须是这个名字）
- **格式**：JPG, PNG 或其他常见图片格式
- **尺寸建议**：300x300 像素以上，正方形最佳
- **文件大小**：建议不超过 500KB

## 如何添加头像

### 方法一：通过访达（Finder）

1. 找到附件中的 `lzp.jpg` 文件
2. 复制该文件
3. 打开博客文件夹 `icoolmedia.github.io`
4. 进入 `assets/img/` 目录
5. 粘贴图片文件

### 方法二：使用终端命令

```bash
# 假设你的头像在下载文件夹
cp ~/Downloads/lzp.jpg /Users/ufo/workspace/demos/icoolmedia.github.io/assets/img/

# 或者从当前位置复制
cp /path/to/lzp.jpg ./assets/img/
```

## 确认头像已设置

头像路径已在配置文件中设置为：`/assets/img/lzp.jpg`

只要你把 `lzp.jpg` 放到这个目录下，重启博客服务器后就能看到头像了！

---

💡 **提示**：如果你的头像文件不叫 `lzp.jpg`，可以重命名，或者修改 `_config.yml` 文件中的 `avatar:` 配置。
