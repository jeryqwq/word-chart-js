##  3D词云图

File           |  % Stmts | % Branch |  % Funcs |  % Lines | Uncovered Line #s |
---------------|----------|----------|----------|----------|-------------------|
All files      |    62.69 |       60 |    52.63 |    61.02 |                   |
 src           |    40.48 |       40 |       25 |    41.03 |                   |
  WordChart.ts |    40.48 |       40 |       25 |    41.03 |... 63,66,67,69,71 |
 src/helper    |      100 |      100 |      100 |      100 |                   |
  constant.ts  |      100 |      100 |      100 |      100 |                   |
  utils.ts     |      100 |      100 |      100 |      100 |                   |

### 纯js开发，无任何第三方依赖
### 基于函数式编程，可在原库上追加自己的业务
### 扩展性强，可自定义追加动画和其他数据
### TS构建，丰富的测试用例
### API
### 数据格式
默认配置：
```ts
const config = {
  el: document.querySelector('#app'),
  data: [
    {
      name: 'node1',
      value: 'node1',

    }
    ...
  ],
  config: {
    fontSizeRange: [12, 24],
    renderFn?:() => HTMLELEMENT | HTMLString,
    speed: 50,
    autoSuit: true, // 自动适配试图
    
    ...
  },
  lifeCycle: {
    beforeSacn: ({item, index, instance}) => ({item, index, instance}),
    afterScan: ({item, index, instance}) => ({item, index, instance}),
    effect: ({item, index, instance}) => void
  }
}
```