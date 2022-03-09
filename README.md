# physicsjs_es6
用es6重构老版本的physicsjs，使其能够在vue+threejs项目中正常运行。
# 安装（stepup）
克隆下载physicsjs_es6文件夹到你的项目中，然后如下引入使用
```javascript
export const THREE = require('three')
import physijs from '/your_path/physi_es6.js'
export const Physic = physijs(THREE) // 这里要执行方法并传入THREE对象，否则无法正常使用
Physic.scripts.worker = '/your_path/physijs_worker.js' // 这里的路径需要注意，要按静态文件引入，所以要把文件放在vue项目中的public文件夹里面
Physic.scripts.ammo = '/your_path/ammo.js' // 这里的路径需要注意，要按静态文件引入，所以要把文件放在vue项目中的public文件夹里面

```
