# deeplx-pro


[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Fxiaozhou26%2Fdeeplx-pro&env=DL_SESSION&project-name=deeplx-pro&repository-name=deeplx-pro)


## 安装部署

```bash
docker run -d --name deeplx-pro -p 9000:9000 -e DL_SESSION="40ef9830-ced3-4f4b-b391-35b98479110f" xiaoxiaofeihh/deeplx-pro:latest
```




## 使用方法

F12打开开发者控制台，然后按照图片复制的cookie的dl_session。
![DeepL翻译API示例代码](https://jsd.cdn.zzko.cn/gh/xiaozhou26/tuph@main/images/2024-03-07%20120245.png)


1. 替换代码中的 `cookie` 变量为你自己的 DeepL Pro cookie。
2. 运行代码，启动 Express 服务器。
3. 使用 POST 请求向 `http://localhost:9000/translate` 发送翻译请求，请求体包含以下字段：
   - `text`：要翻译的文本
   - `source_lang`：源语言（可选，默认为 'AUTO'）
   - `target_lang`：目标语言（可选，默认为 'ZH'）
4. 服务器将返回翻译结果的 JSON 响应。

## 注意事项

- 请不要频繁发送大量请求，否则可能会被 DeepL 暂时阻止 IP。
- 本代码仅供学习和参考，请勿用于商业用途。
- 使用 DeepL 时，请遵守其使用条款和限制。
