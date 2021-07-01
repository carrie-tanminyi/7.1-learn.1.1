### STEP 1：Clone git 地址并安装到 WebStorm
1.在 Github 点击 Code 复制 git 地址
![image.png](https://intranetproxy.alipay.com/skylark/lark/0/2020/png/289367/1598875861076-c0c77360-0447-43d0-9743-bd3d7209ae12.png#height=1037&id=BzMHw&margin=%5Bobject%20Object%5D&name=image.png&originHeight=2074&originWidth=3578&originalType=binary&ratio=1&size=1498207&status=done&style=none&width=1789)


:::info
出现此情况时，需要点击 HTTPS，SSH 是无法 clone 的
:::
![image.png](https://intranetproxy.alipay.com/skylark/lark/0/2020/png/2136/1598876573031-7253cdde-5d4b-42b6-bca8-21617b5de237.png#height=919&id=VuOVH&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1838&originWidth=3572&originalType=binary&ratio=1&size=1483601&status=done&style=none&width=1786)
2.打开 WebStorm 点击 Get from Version Control
![image.png](https://intranetproxy.alipay.com/skylark/lark/0/2020/png/289367/1598875879931-5789ac5c-82b8-4bc8-96e3-17e35b6e2702.png#height=500&id=ROusL&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1000&originWidth=1582&originalType=binary&ratio=1&size=581840&status=done&style=none&width=791)
3.在 URL 地址处粘贴刚才复制的内容，然后点击 clone 
![image.png](https://intranetproxy.alipay.com/skylark/lark/0/2020/png/289367/1598876091478-0dbffdbd-3e2c-4a3f-a30a-31fc4e42d53d.png#height=464&id=rJd3p&margin=%5Bobject%20Object%5D&name=image.png&originHeight=928&originWidth=1492&originalType=binary&ratio=1&size=394399&status=done&style=none&width=746)
4.在新打开的页面点击左下角的 Terminal ，输入下方内容并回车
```
sudo npm install tnpm -g --registry=http://registry.npm.alibaba-inc.com
```
​

![image.png](https://intranetproxy.alipay.com/skylark/lark/0/2020/png/289367/1598876164624-25399429-21be-448f-b83e-993293c8d57a.png#height=1117&id=MNt2A&margin=%5Bobject%20Object%5D&name=image.png&originHeight=2234&originWidth=3576&originalType=binary&ratio=1&size=1655419&status=done&style=none&width=1788)
5.输入电脑开机密码并回车，出现类似下方的内容即代表安装成功
```
“added 1690 packages from 674 contributors and audited 1692 packages in 195.281s”
```


![image.png](https://intranetproxy.alipay.com/skylark/lark/0/2020/png/289367/1598879618739-a988caeb-8dac-4dbd-8dd5-7b7f3c2eb74f.png#height=1119&id=kqO0q&margin=%5Bobject%20Object%5D&name=image.png&originHeight=2238&originWidth=3580&originalType=binary&ratio=1&size=3057563&status=done&style=none&width=1790)
![image.png](https://intranetproxy.alipay.com/skylark/lark/0/2020/png/289367/1598876583045-52ee57ed-bba2-4359-99fb-5ce35f804355.png#height=1118&id=kJzUq&margin=%5Bobject%20Object%5D&name=image.png&originHeight=2236&originWidth=3582&originalType=binary&ratio=1&size=2166473&status=done&style=none&width=1791)
6.输入 tnpm i，出现类似下方内容代表安装成功
![image.png](https://intranetproxy.alipay.com/skylark/lark/0/2020/png/289367/1598879799219-3a173d52-c0f6-4162-9ce9-9926fca47f2c.png#height=1116&id=evWRt&margin=%5Bobject%20Object%5D&name=image.png&originHeight=2232&originWidth=3578&originalType=binary&ratio=1&size=3407075&status=done&style=none&width=1789)


7.双击“release:local"打包到本地，检查是否可用
![image.png](https://intranetproxy.alipay.com/skylark/lark/0/2020/png/289367/1598876715162-df3754d9-31bf-4a23-a052-2667797a2783.png#height=1117&id=hH1tc&margin=%5Bobject%20Object%5D&name=image.png&originHeight=2234&originWidth=3574&originalType=binary&ratio=1&size=2159489&status=done&style=none&width=1787)
> 如果需要卸载，在 Termianl 输入“ sudo npm uninstall -g tnpm"

![image.png](https://intranetproxy.alipay.com/skylark/lark/0/2020/png/289367/1598879417358-49877670-0e87-4b03-8ab4-a68f3680b04c.png#height=1115&id=JAnah&margin=%5Bobject%20Object%5D&name=image.png&originHeight=2230&originWidth=3578&originalType=binary&ratio=1&size=2983146&status=done&style=none&width=1789)




### STEP 2：基于clone git 结构，将原有代码调整到最新结构中
1、首先找到 TextHeight.ts 文件，然后复制一个 ts 文件后，重新命名；复制成功后左侧的 ts 文件会显示绿色。
![image.png](https://intranetproxy.alipay.com/skylark/lark/0/2020/png/2136/1598881101626-607db91b-be4e-4f83-81c2-8a2e9b3c94ba.png#height=919&id=LctnQ&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1838&originWidth=3334&originalType=binary&ratio=1&size=2525917&status=done&style=none&width=1667)


2、打开之前本地已有代码的 WS 文件，然后将原有的 Rule 规则复制替换到此框中。
![image.png](https://intranetproxy.alipay.com/skylark/lark/0/2020/png/2136/1598880794903-2625db19-456d-4215-b64c-d0f4d5787633.png#height=1097&id=aBAxh&margin=%5Bobject%20Object%5D&name=image.png&originHeight=2194&originWidth=3348&originalType=binary&ratio=1&size=3505261&status=done&style=none&width=1674)


3、原有的规则名称是「TextHeightFn」，为了保持统一且易读性，可 Shift +fn+F6 全局调整规则名称：
将 TextHeightFn 改成 ruleFn；将 TextHeight 改成 Rule
![image.png](https://intranetproxy.alipay.com/skylark/lark/0/2020/png/2136/1598881445292-dbe228a8-80a8-4c41-9eb6-58b0433fb35e.png#height=1097&id=AyqW1&margin=%5Bobject%20Object%5D&name=image.png&originHeight=2194&originWidth=3348&originalType=binary&ratio=1&size=3167302&status=done&style=none&width=1674)
4、复制代码后，接下来修改 ts 文件里的 context.utils.repot、title、identifier 、description的名称。
![image.png](https://intranetproxy.alipay.com/skylark/lark/0/2020/png/2136/1598881968050-432757bc-e7e2-4973-a0d3-5075171facc5.png#height=1097&id=rkWyc&margin=%5Bobject%20Object%5D&name=image.png&originHeight=2194&originWidth=3348&originalType=binary&ratio=1&size=3187609&status=done&style=none&width=1674)
5、再找到 rule 下 index.ts 文件，option +d 复制一条代码，然后重命名蓝色框信息，建议和具体 Rule 名字保持一致。可直接 option+s 快速选择。
![image.png](https://intranetproxy.alipay.com/skylark/lark/0/2020/png/2136/1598882105603-cfe917de-470c-4e27-ac3b-1413a1d0faa0.png#height=1097&id=FkYJf&margin=%5Bobject%20Object%5D&name=image.png&originHeight=2194&originWidth=3348&originalType=binary&ratio=1&size=2149901&status=done&style=none&width=1674)
最快的方式，直接 option+s 快速选择，选择刚刚的 ts 文件
![image.png](https://intranetproxy.alipay.com/skylark/lark/0/2020/png/2136/1598882160098-7435dd3d-7668-4b18-b78a-1a1771c826a1.png#height=181&id=catAn&margin=%5Bobject%20Object%5D&name=image.png&originHeight=362&originWidth=1930&originalType=binary&ratio=1&size=95609&status=done&style=none&width=965)


6、找到 _AssistantPackage _的 index.ts 文件，然后在 impot 上输入「，」，并 option + s 选择对应规则；然后在 rules 下 option +d 复制多条规则，并 option + s 选择对应规则![image.png](https://intranetproxy.alipay.com/skylark/lark/0/2020/png/2136/1598882369752-6eec973d-66f4-4a84-9820-cbbc92a36092.png#height=1097&id=tL0Mf&margin=%5Bobject%20Object%5D&name=image.png&originHeight=2194&originWidth=3348&originalType=binary&ratio=1&size=3028301&status=done&style=none&width=1674)


7、package > release:local 打包，看下是否打包成功。
![image.png](https://intranetproxy.alipay.com/skylark/lark/0/2020/png/2136/1598882523708-7a04d28f-cb66-4188-b4fa-92359a2ec350.png#height=1097&id=eNZFj&margin=%5Bobject%20Object%5D&name=image.png&originHeight=2194&originWidth=3348&originalType=binary&ratio=1&size=2598226&status=done&style=none&width=1674)


8、打包成功后，去到 Sketch 文件中安装助理。
:::info
知识点复习：如何安装小助理

- 打开 Sketch 点击 【助理】按钮（需要 Sketch V68 及以上）；
- 在打开的界面中点击右上角的【⚙️ -管理助理-从存档添加...】；
- 然后选择上面生成的 `sketch-assistant-template-1.0.0.tgz` 压缩包进行加载；
- 最后点击【保存】。
:::


![image.png](https://intranetproxy.alipay.com/skylark/lark/0/2020/png/2136/1598882756624-ea9c18fc-3dd9-4f4a-8a0d-43411f37ce06.png#height=1069&id=fO65W&margin=%5Bobject%20Object%5D&name=image.png&originHeight=2138&originWidth=3584&originalType=binary&ratio=1&size=592650&status=done&style=none&width=1792)
### 
### STEP 3：合并本地代码
1.command + K，输入 commit message，然后点击 commit，command+option+g 即可唤起 moji 表情
> commit message 格式：标题+内容（必须为英文）
> 标题分类：
> - type: commit 的类型
> - feat: 新特性
> - fix: 修改问题
> - refactor: 代码重构
> - docs: 文档修改
> - style: 代码格式修改, 注意不是 css 修改
> - test: 测试用例修改
> - chore: 其他修改, 比如构建流程, 依赖管理.
> 


> 作者：阿里南京技术专刊
> 链接：[https://juejin.im/post/6844903606815064077](https://juejin.im/post/6844903606815064077)
> 来源：掘金
> 著作权归作者所有。商业转载请联系作者获得授权，非商业转载请注明出处。

![image.png](https://intranetproxy.alipay.com/skylark/lark/0/2020/png/289367/1598881158979-9933f94d-3320-438f-b6f7-56d02cf20043.png#height=1119&id=XS1KC&margin=%5Bobject%20Object%5D&name=image.png&originHeight=2238&originWidth=3582&originalType=binary&ratio=1&size=3065862&status=done&style=none&width=1791)
💡 小 tips：安装小插件，在 commit message 前带出 emoji 表情 😊
![image.png](https://intranetproxy.alipay.com/skylark/lark/0/2020/png/289367/1598960251018-7e342628-a61a-40c0-9004-4fbfa5212a51.png#height=1009&id=dcivM&margin=%5Bobject%20Object%5D&name=image.png&originHeight=2018&originWidth=3582&originalType=binary&ratio=1&size=2755202&status=done&style=none&width=1791)
![image.png](https://intranetproxy.alipay.com/skylark/lark/0/2020/png/289367/1598958864304-255c1e7d-3621-4b6f-adb4-5c75a5800dc1.png#height=1037&id=LiPcS&margin=%5Bobject%20Object%5D&name=image.png&originHeight=2074&originWidth=3582&originalType=binary&ratio=1&size=3355355&status=done&style=none&width=1791)
![image.png](https://intranetproxy.alipay.com/skylark/lark/0/2020/png/289367/1598958887270-b1310bc2-eea7-40a5-b145-e23cb54953a8.png#height=1039&id=BftnM&margin=%5Bobject%20Object%5D&name=image.png&originHeight=2078&originWidth=3578&originalType=binary&ratio=1&size=3596183&status=done&style=none&width=1789)
![image.png](https://intranetproxy.alipay.com/skylark/lark/0/2020/png/289367/1598958913882-67e097ea-de8a-47b0-b80a-3cd26846fb60.png#height=1032&id=qp47P&margin=%5Bobject%20Object%5D&name=image.png&originHeight=2064&originWidth=3582&originalType=binary&ratio=1&size=2909696&status=done&style=none&width=1791)
![image.png](https://intranetproxy.alipay.com/skylark/lark/0/2020/png/289367/1598958938079-7eb85004-1a6f-463e-b7ac-3472d8da6678.png#height=1036&id=zG2vJ&margin=%5Bobject%20Object%5D&name=image.png&originHeight=2072&originWidth=3578&originalType=binary&ratio=1&size=3308441&status=done&style=none&width=1789)
![image.png](https://intranetproxy.alipay.com/skylark/lark/0/2020/png/289367/1598959052146-215f178a-81f5-4bb1-9453-c23df0120191.png#height=1010&id=QA9g5&margin=%5Bobject%20Object%5D&name=image.png&originHeight=2020&originWidth=3582&originalType=binary&ratio=1&size=3416484&status=done&style=none&width=1791)
![image.png](https://intranetproxy.alipay.com/skylark/lark/0/2020/png/2136/1598959121498-3e0e589f-a77a-4cbc-b2ad-15efbadadad5.png#height=1097&id=MkdTU&margin=%5Bobject%20Object%5D&name=image.png&originHeight=2194&originWidth=3348&originalType=binary&ratio=1&size=3468203&status=done&style=none&width=1674)
![image.png](https://intranetproxy.alipay.com/skylark/lark/0/2020/png/289367/1598959155126-52536977-3617-4595-8d8d-76c45595596e.png#height=1010&id=QsguY&margin=%5Bobject%20Object%5D&name=image.png&originHeight=2020&originWidth=3578&originalType=binary&ratio=1&size=3308814&status=done&style=none&width=1789)
把别人的仓库复制到自己的仓库里
![image.png](https://intranetproxy.alipay.com/skylark/lark/0/2020/png/289367/1598959238131-e5966a85-8712-47d9-8207-00a8026814d7.png#height=1074&id=MlXFo&margin=%5Bobject%20Object%5D&name=image.png&originHeight=2148&originWidth=3576&originalType=binary&ratio=1&size=1511138&status=done&style=none&width=1788)
### 
### STEP 4：修改远程仓库的地址到自己仓库的地址
![image.png](https://intranetproxy.alipay.com/skylark/lark/0/2020/png/289367/1598959385931-6f2ea9f4-a7e1-4905-a70f-c82ffcab5067.png#height=1041&id=a7eqs&margin=%5Bobject%20Object%5D&name=image.png&originHeight=2082&originWidth=3582&originalType=binary&ratio=1&size=3604492&status=done&style=none&width=1791)
![image.png](https://intranetproxy.alipay.com/skylark/lark/0/2020/png/289367/1598959452344-173b839f-a155-4580-9c1f-7e48db2291af.png#height=1071&id=D7Sj2&margin=%5Bobject%20Object%5D&name=image.png&originHeight=2142&originWidth=3580&originalType=binary&ratio=1&size=1613134&status=done&style=none&width=1790)
![image.png](https://intranetproxy.alipay.com/skylark/lark/0/2020/png/289367/1598959531236-37ac7317-1247-41b4-9935-7ea39bf84b9b.png#height=1039&id=pFxVU&margin=%5Bobject%20Object%5D&name=image.png&originHeight=2078&originWidth=3582&originalType=binary&ratio=1&size=1490821&status=done&style=none&width=1791)
合并请求
在主仓库里
![image.png](https://intranetproxy.alipay.com/skylark/lark/0/2020/png/289367/1598959653994-2f5e9213-aee8-4b68-934b-174215da6b5a.png#height=1015&id=RBLnt&margin=%5Bobject%20Object%5D&name=image.png&originHeight=2030&originWidth=3582&originalType=binary&ratio=1&size=1011261&status=done&style=none&width=1791)
![image.png](https://intranetproxy.alipay.com/skylark/lark/0/2020/png/289367/1598959838022-59d3e9f9-5432-4223-a049-06ac4e280282.png#height=957&id=ebU8D&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1914&originWidth=3582&originalType=binary&ratio=1&size=1640576&status=done&style=none&width=1791)
![image.png](https://intranetproxy.alipay.com/skylark/lark/0/2020/png/289367/1598959952010-bdbe6c0b-6650-426d-9c2b-b36fdaad3295.png#height=1039&id=INul3&margin=%5Bobject%20Object%5D&name=image.png&originHeight=2078&originWidth=3572&originalType=binary&ratio=1&size=1515578&status=done&style=none&width=1786)


### 
### STEP 5：写测试用例
写测试用例可以验证代码规则是否有问题，同时还可以基础测试用例反馈结构，来推导代码规则。


1、目前该文件已有一条 TextHeight 的 test ，复制后，将以下的红色框的名称改成对应的 rules 名称。
![image.png](https://intranetproxy.alipay.com/skylark/lark/0/2020/png/2136/1598969191802-b0d25185-13e4-4176-b84b-4c0d8d2bd6ae.png#height=1094&id=IjvWS&margin=%5Bobject%20Object%5D&name=image.png&originHeight=2188&originWidth=3348&originalType=binary&ratio=1&size=2640514&status=done&style=none&width=1674)


2、复制 TextHeight sketch ，然后在 sketch 中，制作几条正确的和错误的规则案例。
![image.png](https://intranetproxy.alipay.com/skylark/lark/0/2020/png/2136/1598969813656-f7eea4d6-bec1-4eef-a001-38d167ad7319.png#height=504&id=yNSn5&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1008&originWidth=1786&originalType=binary&ratio=1&size=248859&status=done&style=none&width=893)
3、写完测试用例后， 点击「Run 规则」 跑一下，看测试用例和 sketch 的规则是否一致？
![image.png](https://intranetproxy.alipay.com/skylark/lark/0/2020/png/2136/1599052411151-6250325f-28a6-40d0-8f06-0889ee671cef.png#height=1097&id=nv1BA&margin=%5Bobject%20Object%5D&name=image.png&originHeight=2194&originWidth=3348&originalType=binary&ratio=1&size=2675595&status=done&style=none&width=1674)
4、expected 是期望系统提示出错的数量，如果 sketch 的规则里做了一条错误规则，则此处应填「1」。Run 完后底部显示就成功了。
![image.png](https://intranetproxy.alipay.com/skylark/lark/0/2020/png/2136/1599052323274-e12fefc6-3c79-46a1-a573-47f764f1d766.png#height=1097&id=pZMeW&margin=%5Bobject%20Object%5D&name=image.png&originHeight=2194&originWidth=3348&originalType=binary&ratio=1&size=2806701&status=done&style=none&width=1674)
5、接下里，点击 package 打包一下，再到 sketch 看下最终实现效果。
​

如何引用
