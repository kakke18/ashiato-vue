<template>
  <v-card-text>
    <vue-good-table
      class="award-table"
      :columns="columns"
      :rows="rows"
      :fixed-header="true"
      :pagination-options="{
        enabled: true,
        perPageDropdown: [5, 10, 30]
      }"
      :sort-options="{
        enabled: false
      }"
    />
  </v-card-text>
</template>

<script>
import 'vue-good-table/dist/vue-good-table.css'
import { VueGoodTable } from 'vue-good-table'
export default {
  components: {
    VueGoodTable
  },
  data() {
    return {
      columns: [
        {
          label: '年月日',
          field: 'date',
          type: 'string',
          thClass: 'text-center',
          tdClass: 'text-left'
        },
        {
          label: '内容',
          field: 'content',
          type: 'string',
          html: true,
          thClass: 'text-center',
          tdClass: 'text-left'
        }
      ],
      rows: [
        {
          date: '2020年3月6日，7日',
          content:
            '<b>HAIシンポジウム2020</b><br>口頭発表(新型コロナウイルスの影響で発表は中止)．'
        },
        {
          date: '2020年2月29日，3月1日',
          content:
            '<b>第9回 サイエンス・インカレ</b><br>書類審査に通過し口頭発表のファイナリストに選出(新型コロナウイルスの影響で発表は中止)．'
        },
        {
          date: '2019年12月12日',
          content:
            '<b>成績優秀者 表彰式</b><br>静岡大学における成績優秀者賞を受賞．'
        },
        {
          date: '2019年10月6日-10日',
          content: '<b>HAI2019</b><br>国際会議にて口頭発表及びポスター発表．'
        },
        {
          date: '2019年8月21日',
          content:
            '<b>Hack U 2019 NAGOYA</b><br>Yahoo!JAPAN主催の学生ハッカソンに参加．'
        },
        {
          date: '2019年3月2日，3日',
          content:
            '<b>第8回 サイエンス・インカレ</b><br>ファイナリストとして口頭発表．審査員特別賞を受賞．記事は<a href="http://www.inf.shizuoka.ac.jp/news/detail.html?CN=154274" target="_blank">こちら</a>．'
        },
        {
          date: '2018年12月15日',
          content:
            '<b>地域づくりin静岡～アプリで実現する地方創生～ ハッカソン</b><br>静岡大学にてハッカソンに参加．審査員特別賞を受賞．記事は<a href="http://www.inf.shizuoka.ac.jp/news/detail.html?CN=154258" target="_blank">こちら</a>．'
        },
        {
          date: '2018年9月29日',
          content:
            '<b>地域づくりin静岡～アプリで実現する地方創生～ アイデアソン</b><br>静岡大学にてアイデアソンに参加．ユニーク・アイデア賞を受賞．記事は<a href="http://www.inf.shizuoka.ac.jp/news/detail.html?CN=154235" target="_blank">こちら</a>．'
        },
        {
          date: '2018年3月16日',
          content:
            '<b>松江高専 卒業式</b></br>電気情報学会賞，功労賞，優秀成績賞，及び優秀卒業学生表彰．'
        },
        {
          date: '2018年3月2日，3日',
          content:
            '<b>第39回 ゲーム情報学研究会</b><br>東京大学にて口頭発表．若手奨励賞を受賞．記事は<a href="https://www.matsue-ct.jp/m/index.php/215-all-topics/topics201803/2463-tp20180327" target="_blank">こちら</a>．'
        },
        {
          date: '2017年3月25日',
          content:
            '<b>第2回 スモウルビー甲子園 トークセッション</b><br>まつもとゆきひろさん，池澤あやかさんとのトークセッションに参加．'
        },
        {
          date: '2017年1月6日-8日',
          content:
            '<b>第58回 プログラミング・シンポジウム</b><br>ラフォーレ倶楽部伊東にてポスター発表．'
        },
        {
          date: '2016年11月26日，27日',
          content:
            '<b>RESAS-APIでチャレンジ！島根の地方創生ハッカソン</b><br>RESAS-APIを用いたハッカソンに参加．機械学習に触れる．'
        },
        {
          date: '2016年9月24日',
          content:
            '<b>オープンソースカンファレンス2016 Shimane</b><br>学生ゾーン展示ブースにて個人出展及び団体出展．記事は<a href="https://www.ospn.jp/osc2016-shimane/modules/article/article.php?articleid=10/" target="_blank">こちら</a>．'
        },
        {
          date: '2016年9月17日',
          content:
            '<b>スモウルビー甲子園体験セミナー</b><br>松江オープンソースラボにて講演．'
        },
        {
          date: '2016年9月10日，11日',
          content:
            '<b>ひやおろしGO ハッカソン</b><br>古民家「風神坊」にて開催のRailsを用いたハッカソンに参加．'
        },
        {
          date: '2016年8月29日-9月9',
          content:
            '<b>NaCl インターンシップ</b><br>ネットワーク応用通信研究所のインターンシップに参加．'
        },
        {
          date: '2016年8月21日',
          content:
            '<b>第51回 全国高専大会</b><br>100m平泳ぎ1位，200m平泳ぎ1位．100m平泳ぎ3年連続優勝により全国高等専門学校体育大会特別表彰．記事は<a href="https://www.matsue-ct.jp/m/index.php/198-all-topics/topics201610/2086-tp20161020" target="_blank">こちら</a>．'
        },
        {
          date: '2016年3月26日',
          content:
            '<b>第1回 スモウルビー甲子園</b><br>決勝大会に出場し，優勝．記事は<a href="https://www.matsue-ct.jp/it/index.php/44-topics/topics2015b/277-topics20160327" target="_blank">こちら</a>．'
        },
        {
          date: '2016年2月29日-3月4日',
          content:
            '<b>Ruby合宿 2016春</b><br>Arduinoを用いたゲームを開発し，発表．'
        },
        {
          date: '2016年2月21日',
          content:
            '<b>第164回 中国室内水泳競技大会</b><br>高校最後の水泳大会．優秀選手賞を受賞．'
        },
        {
          date: '2016年1月11日',
          content:
            '<b>松江市 選手表彰式</b><br>松江市における水泳の優秀選手賞を受賞．'
        },
        {
          date: '2015年8月30日',
          content:
            '<b>第50回 全国高専大会</b><br>100m平泳ぎ1位，200m平泳ぎ1位．'
        },
        {
          date: '2015年7月12日',
          content:
            '<b>平成27年度 島根県選手権水泳競技大会</b><br>100m平泳ぎ，及び200m平泳ぎで県選手権(県内1位)を獲得．記事は<a href="http://shimane-suiren.jp/publics/index/1/detail=1/b_id=5/r_id=129#block5-129" target="_blank">こちら</a>．'
        },
        {
          date: '2014年8月24日',
          content:
            '<b>第49回 全国高専大会</b><br>100m平泳ぎ1位，200m平泳ぎ2位．'
        },
        {
          date: '2014年7月13日',
          content:
            '<b>平成26年度 島根県選手権水泳競技大会</b><br>100m平泳ぎで県選手権(県内1位)を獲得．記事は<a href="http://shimane-suiren.jp/publics/index/1/detail=1/b_id=5/r_id=90#block5-90" target="_blank">こちら</a>．'
        },
        {
          date: '2012年11月28日',
          content:
            '<b>しまね調べ学習プレゼンテーションコンテスト</b><br>中学校代表で口頭発表し，優秀賞を受賞．'
        },
        {
          date: '2011年9月2日',
          content:
            '<b>平成23年度 少年の主張 松江大会</b><br>中学校代表で口頭発表し，優秀賞を受賞．'
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
.award-table ::v-deep .vgt-table {
  font-size: 10px;
}
@media only screen and (min-width: 651px) {
  .award-table ::v-deep .vgt-table {
    font-size: 16px;
  }
}
</style>
