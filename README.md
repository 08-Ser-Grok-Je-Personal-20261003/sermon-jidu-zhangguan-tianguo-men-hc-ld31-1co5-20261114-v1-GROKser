# 基督掌管天国的门 · 林前5 · 海德堡要理问答主日31
# Christ Holds the Keys of the Kingdom · 1 Corinthians 5 · Heidelberg Catechism Lord's Day 31

## 线上链接 / Live links

- GitHub Pages: https://08-ser-grok-je-personal-20261003.github.io/sermon-jidu-zhangguan-tianguo-men-hc-ld31-1co5-20261114-v1-GROKser/
- Surge: https://jidu-zhangguan-tianguo-men-hc-ld31-1co5-20261114-v1-grokser.surge.sh
- Repository: https://github.com/08-Ser-Grok-Je-Personal-20261003/sermon-jidu-zhangguan-tianguo-men-hc-ld31-1co5-20261114-v1-GROKser

讲题：基督掌管天国的门。要点：① 福音打开门　② 纪律关上门　③ 管教为挽回。
诗歌只列编号：韵诗24篇 · 韵诗25篇1–3节 · 韵诗第1篇 · 圣诗第16首 · 圣诗第9首。

静态多页网站（HTML / CSS / 原生 JS，无外部库）。版式与对比度沿用主日30模板的 v1.1 配色。Surge 由协调员在自己的电脑发布；本仓库不放 CNAME，也不放登录信息。

## 结构 / Structure

| 文件 | 内容 |
|---|---|
| `index.html` | 总入口、一句话总结、三点默想、站点地图、三条线上链接 |
| `sermon.html` | 完整讲章、背景、四个闭环、18道讨论题、逐节大意、信条原文 |
| `keys.html` | 天国的钥匙与纪律：开关图、步骤、对照表、受害保护、1563/1570界线 |
| `creeds-read.html` | 三大信经阅读与背诵 |
| `forms-read.html`, `hc.html`, `belgic.html`, `dort.html` | 三项联合信条全文 |
| `compare.html` | 三信经与三信条比较：相同、差别、各自的问题、为何是三份 |
| `memorize.html` | 闪卡、填空、测验、打印摘要 |
| `resources.html` | 出处 |
| `corpus/` | 信经与信条 JSON |
| `build.py` | 由 `src/` 与 `corpus/` 生成页面 |
| `verify_verbatim.py` | 逐字校验与漏引扫描 |

## 如何重新生成

```bash
python3 build.py
python3 verify_verbatim.py
python3 tools/check_links.py
python3 tools/qa.py /tmp/shots-ld31 --shots
python3 tools/contrast_audit.py /tmp/contrast-ld31
```

引文指令如 `{{HC 83}}`、`{{BC 32}}`、`{{DORT 5 5}}` 只从 `corpus/` 取文。圣经讲解标为“大意”。

## 保留与限制

- 地图标明为示意图。不画尼禄后来才动工、并未完成的运河，也不标未经复核的经纬度。
- 林前5:5保留四种读法。加尔文的“败坏肉体”是今世的缓和责罚，不是“罪性被治死”。不采纳咒诅致死。
- 林后2章那人是否即林前5章的人，不定案。
- 1563年要理与1570年7月13日敕令分开。敕令是折中，不是日内瓦式长老会的完全建立。文献自己说经过尚未充分厘清。
- 圣诗与韵诗只列编号，不转录歌词。
- 闪卡进度只存在访问者浏览器的 localStorage。
