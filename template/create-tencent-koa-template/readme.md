# create-tencent-koa-template

## 使用
1. 安装serverless
```
npm i -g serverless
```
2. 修改`.env`
```
TENCENT_SECRET_ID=xxx
TENCENT_SECRET_KEY=xxx
```
3. 修改`serverless.yml`
```yml
# serverless.yml

koa:
  component: 'cmux-tencent-koa'
  inputs:
    region: ap-beijing
    functionName: $functionName
    tags:
      ux: webtest1
```
4. 安装依赖
```
yarn
```
5. 发布
```
sls --debug
```