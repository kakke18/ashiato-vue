<template>
  <v-card-text>
    <v-list-item v-for="item in items" :key="item.title">
      <v-list-item-content class="text-left">
        <v-list-item-title v-text="item.title" />
        <v-list-item-subtitle
          v-for="content in item.content"
          :key="content"
          v-text="content"
        />
      </v-list-item-content>
    </v-list-item>
  </v-card-text>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          title: '強化学習を通したクリーチャによる協調行動の自動獲得',
          content: ['HAIシンポジウム2020, Mar. 2020', '高田 亮介, 竹内 勇剛']
        },
        {
          title:
            'ニューロエボリューションによるエージェントの立位獲得過程に関する研究',
          content: [
            '第8回浜松アカデミックカンファレンス, Feb. 2020',
            '山田 雅敏, 高田 亮介, 竹内 勇剛'
          ]
        },
        {
          title:
            'Design of Cooperative Interaction between Humans and AI Creatures through Reinforcement Learning',
          content: ['HAI 2019, Oct. 2019', 'Ryosuke Takata, Yugo Takeuchi']
        },
        {
          title:
            'Design of Cooperative Interaction between Humans and Agents through Reinforcement Learning',
          content: [
            'Next Generation Human-Agent Interaction Workshop, Oct. 2019',
            'Ryosuke Takata, Yugo Takeuchi'
          ]
        },
        {
          title:
            '無限1UPを題材としたアクションゲームの裏技を発見する自己学習手法の提案(若手奨励賞 受賞)',
          content: [
            '第39回情報処理学会ゲーム情報学研究会, pp.1-7, Mar. 2018',
            '高田 亮介, 橋本 剛',
            '(若手奨励賞 受賞)'
          ]
        },
        {
          title: '自己学習で裏技を発見するアクションゲームAIの研究',
          content: [
            '松江工業高等専門学校卒業論文, pp.1-27, Feb. 2018',
            '高田 亮介, 橋本 剛'
          ]
        },
        {
          title: '第1回スモウルビー甲子園優勝プログラムと将来の展望',
          content: [
            '第58回プログラミング・シンポジウム予稿集, pp.81-83, Jan. 2017',
            '高田 亮介, 加藤 聡'
          ]
        }
      ]
    }
  }
}
</script>
