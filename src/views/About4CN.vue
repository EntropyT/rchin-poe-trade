<template>
<div class="about">
  <div style="padding:5px 30px;">
    <b-card-group deck>
      <b-card border-variant="primary" header="POE 查价工具 v1.312.4.1" header-bg-variant="primary" header-text-variant="white" align="center">
        <b-card-text>作者：EntropyT | 原作者：rChinnnn</b-card-text>
        <b-card-text>
          <b-button @click="openLink(`https://github.com/EntropyT/EntropyT-POE-Trade4CN`)" size="sm" variant="outline-primary" class="mb-2">
            历史版本请点我
          </b-button>
        </b-card-text>
      </b-card>
    </b-card-group>
  </div>
  <div style="padding:5px 30px;">
    <b-card-group deck>
      <b-card border-variant="danger" header="免责申明" header-bg-variant="danger" header-text-variant="white" align="center">
        <b-card-text>
          <h5>使用此程序请自行承担所有可能后果和风险</h5>
        </b-card-text>
        <b-card-text>此程序并没有修改任何内容和游戏内容</b-card-text>
        <b-card-text>运作原来为抓取 POE 游戏内对物品复制的文字进行解析，以便快速查价</b-card-text>
        <b-card-text>调用的 API 皆为官方公开资源，请勿于短时间内快速搜索造成服务器负担</b-card-text>
      </b-card>
    </b-card-group>
  </div>
  <div style="padding:5px 30px;">
    <b-card-group deck>
      <b-card border-variant="dark" header="使用说明" header-bg-variant="dark" header-text-variant="white" align="center">
        <b-card-text>1. 点此页上面的 HOME 页签</b-card-text>
        <b-card-text>2. 切换至游戏国际服界面</b-card-text>
        <b-card-text>3. 将鼠标停在物品上，按下 Ctrl+C </b-card-text>
        <b-card-text>4. 程序将自动判断此次搜索物品进行查价 </b-card-text>
        <b-card-text>
          <b-button @click="openLink(`https://github.com/EntropyT/EntropyT-POE-Trade4CN/blob/master/README.md`)" size="sm" variant="outline-primary" class="mb-2">
            详细使用说明及基础搜索设定请点我
          </b-button>
        </b-card-text>
      </b-card>
    </b-card-group>
  </div>
  <div style="padding:5px 30px;">
    <b-card-group deck>
      <b-card border-variant="dark" header="热键功能" header-bg-variant="dark" header-text-variant="white" align="center">
        <table class="table table-sm">
          <thead class="thead-light">
            <tr>
              <th scope="col">按键</th>
              <th scope="col">功能说明</th>
            </tr>
          </thead>
          <tbody class="hotkey">
            <tr v-for="(item, index) in hotkey" :key="index" style="padding-top: 5px;">
              <td align="left">{{ item.key }}</td>
              <td align="left">{{ item.description }}</td>
            </tr>
          </tbody>
        </table>
        <b-card-text><b style="background-color: lightyellow;">注意事项：所有热键于 POE 游戏窗口内皆无作用！必须在工具窗口内才可以使用</b></b-card-text>
      </b-card>
    </b-card-group>
  </div>
  <div style="padding:5px 30px;">
    <b-card-group deck>
      <b-card border-variant="info" header-bg-variant="info" header-text-variant="white" header="這是免費程式 / 贊助連結" align="center">
        <b-card-text>此程序已在 GITHUB 上开源</b-card-text>
        <b-card-text>欢迎分享给朋友使用</b-card-text>
        <b-card-text>若工具对你有不少帮助，也有余力的话</b-card-text>
        <b-card-text>请作者在开发新功能时喝杯咖啡吧：）</b-card-text>
<!--        <b-card-text>-->
<!--          <b-button @click="openLink(``)" size="sm" variant="outline-primary" class="mb-2">-->
<!--            支付宝 <b-icon icon="credit-card"></b-icon>-->
<!--          </b-button>-->
<!--          <b-card-img src="../assets/pay.jpg">Coffee</b-card-img>-->
<!--        </b-card-text>-->
      </b-card>
    </b-card-group>
  </div>
</div>
</template>

<script>
const {
  clipboard,
  shell
} = require('electron')

export default {
  data() {
    return {
      hotkey: [{
        "key": "F5",
        "description": "程序显示在最上层，并且透明化（可悬浮在POE程序上）"
      }, {
        "key": "F6",
        "description": "程序取消最上层，并取消透明化"
      }, {
        "key": "PageUp",
        "description": "透明化程度 +5%"
      }, {
        "key": "PageDown",
        "description": "透明化程度 -5%"
      }, ]
    }
  },
  methods: {
    openLink(URL) {
      shell.openExternal(URL)
    },
  },
}
</script>

<style>
.card-body {
  padding: 10px !important;
}

.card-text p {
  margin-block-start: 0.5em;
  margin-block-end: 0em;
}

tbody.hotkey>tr>td {
  padding-top: 8px;
  padding-left: 25px;
}
</style>
