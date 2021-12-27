## 奇淫技巧

- [谷歌总是找不到想要的内容？学会这14个技巧，立马就能找到](https://juejin.cn/post/7025750708930478111)

- **快捷变量命名**

  我的做法：

  1. 安装vscode插件 draven的 translate
  
  2. 找到插件代码修改 extension.js
  
  3. 再结果返回处添加
  
     ```javascript
     let res = response.toLowerCase().trim();
     vscode.window.showInformationMessage(`${_text} 翻译成 ${res}`);
     vscode.env.clipboard.writeText(res)
     ```
  
  4. 保存后重启vscode
  
     ![](https://s2.loli.net/2021/12/27/UH7xXQCiIrjGtKb.gif)
