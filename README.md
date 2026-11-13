<div align="center">

# クォン・イゴン / Kwon Leegun

韓国と日本のあいだで働く人のためのツールを作っています。<br>
I build tools for people working between Korea and Japan.<br>
한국과 일본 사이에서 일하는 사람을 위한 도구를 만듭니다.

[![Email](https://img.shields.io/badge/Email-hkys1223%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:hkys1223@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-2daKaizen--gun-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/2daKaizen-gun)
![JLPT](https://img.shields.io/badge/JLPT-N2-E60012?style=flat-square)
![Location](https://img.shields.io/badge/Seoul_→_Kyoto_2027-4285F4?style=flat-square&logo=googlemaps&logoColor=white)

</div>

## About

- 漢城大学（ソウル）コンピュータ工学科 在学中<br>CS student at Hansung University, Seoul
- 2027年から京都府立大学へ交換留学予定。卒業後は日本で働きたいと考えています<br>Exchange student at Kyoto Prefectural University from 2027, planning to work in Japan
- AI とフルスタック開発が中心です<br>Mainly AI and full-stack development
- 日本語 JLPT N2 ・ English ・ 한국어（母語）

日本語を勉強する中で不便だったこと（敬語のメール、祝日のずれ、単語の整理など）を、そのままプロジェクトにしてきました。<br>
Most of these projects started from small problems I ran into while learning Japanese.

## Projects

### KOTONA

ビジネス日本語の文章を入力すると、敬語の丁寧さや遠回しな断り（本音と建前）を判定し、返信案を3パターン提案するアプリです。<br>
Analyzes Japanese business messages for politeness and indirect refusals, and suggests three reply options.

- `Java` `Spring Boot` `Next.js` `TypeScript` `Gemini` `MySQL` `Docker`
- 形態素解析（Kuromoji）のルールと Gemini の判定を組み合わせ、ラベル付きの例文 41 件で精度を確認しています。Gemini の出力は JSON スキーマで固定
- テスト：バックエンド 265 件、フロントエンド 175 件 + E2E 12 件（CI で毎回実行）
- [Demo](https://kotona-web.vercel.app)（サンプルデータで動くデモ版） ・ [kotona-analyzer](https://github.com/2daKaizen-gun/kotona-analyzer) ・ [kotona-web](https://github.com/2daKaizen-gun/kotona-web)

### Pale Blue Code

NASA TESS 衛星の公開データから、まだカタログにない系外惑星を探すアプリです。太陽系の 3D 表示や重力シミュレーションなど、学習用の画面もあります。<br>
Searches public TESS data for uncatalogued exoplanets, with 3D and simulation views for learning.

- `React` `TypeScript` `Three.js` `GLSL` `D3.js` `FastAPI` `Python` `lightkurve`
- TESS セクター 102–106 の小さな恒星 328 個を調べた結果、目立つシグナル 55 件はすべて観測装置由来のノイズで、惑星候補は 0 件でした。恒星ごとにどのサイズまで検出できたかも合わせて記録しています
- テスト：pytest 244 件、vitest 250 件
- [Demo](https://pale-blue-code.vercel.app)（フロントエンドのみ常時公開） ・ [Repository](https://github.com/2daKaizen-gun/pale-blue-code)

### 冴え (Sae)

90秒の反応時間テスト（PVT）で、その日の頭の冴えを 0–100 で記録する iOS アプリです。ウェアラブル端末は使いません。<br>
An iOS app that turns a 90-second reaction-time test into a daily alertness score. No wearable needed.

- `Swift` `SwiftUI` `SwiftData` `HealthKit` `CoreMotion` ・ 日本語 / English / 한국어
- 刺激の表示時刻は `CADisplayLink`、タップは `UITouch.timestamp` から取り、描画の遅れが反応時間に混ざらないようにしました
- スコアは元の測定値から計算をたどれるようにしています。テスト 96 件
- [Repository](https://github.com/2daKaizen-gun/sae)

## その他 / Other

| Project | 内容 / What | Stack |
|---|---|---|
| [SkyWear](https://github.com/2daKaizen-gun/skywear) | 韓国と日本の気温差から、旅行の服装を8段階で提案する Android アプリ<br>Outfit suggestions from the KR–JP temperature gap | `Kotlin` `Jetpack Compose` `Hilt` `Room` |
| [JP-KR Schedule Bridge](https://github.com/2daKaizen-gun/jp-kr-schedule-bridge) | 韓日の祝日を並べて表示し、Gemini でビジネスメールの下書きを作成（[Demo](https://jp-kr-schedule-bridge.vercel.app)）<br>KR/JP holiday calendar with Gemini email drafts | `Next.js` `TypeScript` `Gemini` |
| [JP-Dictionary-Bot](https://github.com/2daKaizen-gun/jp-dict-bot) | 単語を入れると JLPT レベルや IT・ビジネスの例文を付けて Notion に保存<br>Japanese vocabulary notes, synced to Notion | `Python` `Streamlit` `Gemini` `Notion API` |
| [survey-auto-summarizer](https://github.com/2daKaizen-gun/survey-auto-summarizer) | 大学の国際交流プログラムのアンケート（多言語）を集計・要約<br>Summarizes multilingual survey responses from Google Sheets | `Python` `Pandas` `Gemini` `Sheets API` |

## Tech Stack

**Language**
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Java](https://img.shields.io/badge/Java-007396?style=flat-square&logo=openjdk&logoColor=white)
![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white)
![Swift](https://img.shields.io/badge/Swift-F05138?style=flat-square&logo=swift&logoColor=white)

**Frontend**
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-000?style=flat-square&logo=nextdotjs&logoColor=white)
![Three.js](https://img.shields.io/badge/Three.js-000?style=flat-square&logo=threedotjs&logoColor=white)
![D3.js](https://img.shields.io/badge/D3.js-F9A03C?style=flat-square&logo=d3dotjs&logoColor=white)
![Tailwind](https://img.shields.io/badge/Tailwind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)

**Backend / DB**
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)

**Mobile**
![Android](https://img.shields.io/badge/Android-3DDC84?style=flat-square&logo=android&logoColor=white)
![Jetpack Compose](https://img.shields.io/badge/Jetpack_Compose-4285F4?style=flat-square&logo=jetpackcompose&logoColor=white)
![SwiftUI](https://img.shields.io/badge/SwiftUI-F05138?style=flat-square&logo=swift&logoColor=white)

**AI / Data**
![Gemini](https://img.shields.io/badge/Gemini-8E75B2?style=flat-square&logo=googlegemini&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)

**Infra / Tools**
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![AWS](https://img.shields.io/badge/AWS_EC2-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)
![Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000?style=flat-square&logo=vercel&logoColor=white)
![Claude Code](https://img.shields.io/badge/Claude_Code-D97757?style=flat-square&logo=claude&logoColor=white)

**Testing**
![Vitest](https://img.shields.io/badge/Vitest-6E9F18?style=flat-square&logo=vitest&logoColor=white)
![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white)
![pytest](https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white)
![JUnit5](https://img.shields.io/badge/JUnit5-25A162?style=flat-square&logo=junit5&logoColor=white)

## Activity

<div align="center">

<img src="./profile-3d-contrib/profile-season-animate.svg" alt="3D contribution calendar" width="100%">

<br>

<img src="./github-metrics.svg" alt="GitHub metrics" width="100%">

</div>
