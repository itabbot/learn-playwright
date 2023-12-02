# 初始化 Playwright 项目，并体验其基本功能

## 1. 初始化项目

通过官方脚手架生成基本的项目结构，并安装依赖和浏览器内核。

```shell
> npm init playwright@latest

Getting started with writing end-to-end tests with Playwright:
Initializing project in '.'

√ Do you want to use TypeScript or JavaScript? · JavaScript
√ Where to put your end-to-end tests? · tests
√ Add a GitHub Actions workflow? (y/N) · false
√ Install Playwright browsers (can be done manually via 'npx playwright install')? (Y/n) · true

Initializing NPM project (npm init -y)…
Wrote to package.json:
{
  "name": "init",
  "version": "1.0.0"
}

Installing Playwright Test (npm install --save-dev @playwright/test)…
added 3 packages, and audited 4 packages in 26s

Installing Types (npm install --save-dev @types/node)…
added 2 packages, and audited 6 packages in 5s

Downloading browsers (npx playwright install)…

Downloading Chromium 120.0.6099.28 (playwright build v1091) from https://playwright.azureedge.net/builds/chromium/1091/chromium-win64.zip
122 Mb [====================] 100% 0.0s
Chromium 120.0.6099.28 (playwright build v1091) downloaded to C:\xxx\ms-playwright\chromium-1091

Downloading FFMPEG playwright build v1009 from https://playwright.azureedge.net/builds/ffmpeg/1009/ffmpeg-win64.zip
1.4 Mb [====================] 100% 0.0s
FFMPEG playwright build v1009 downloaded to C:\xxx\ms-playwright\ffmpeg-1009

Downloading Firefox 119.0 (playwright build v1429) from https://playwright.azureedge.net/builds/firefox/1429/firefox-win64.zip
80.5 Mb [====================] 100% 0.0s
Firefox 119.0 (playwright build v1429) downloaded to C:\xxx\ms-playwright\firefox-1429

Downloading Webkit 17.4 (playwright build v1944) from https://playwright.azureedge.net/builds/webkit/1944/webkit-win64.zip
46.4 Mb [====================] 100% 0.0s
Webkit 17.4 (playwright build v1944) downloaded to C:\xxx\ms-playwright\webkit-1944

Writing playwright.config.js.
Writing tests\example.spec.js.
Writing tests-examples\demo-todo-app.spec.js.
Writing package.json.

✔ Success! Created a Playwright Test project at D:\xxx\learn-playwright\quick-start\init
```

## 2. 基本功能

运行所有端到端测试

```shell
npx playwright test
```

运行特定文件中的测试

```shell
npx playwright test example
```

启动交互 UI 模式

```shell
npx playwright test --ui
```

仅在 Chrome 上运行测试

```shell
npx playwright test --project=chromium
```

以调试模式运行测试

```shell
npx playwright test --debug
```

使用 Codegen 自动生成测试

```shell
npx playwright codegen
```
