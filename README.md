## **furniture/ form/ family -HPShelf**
***
- Introduction
- About Software
- Working Process
- Development Environment
- Download Generator
- Thinking Note
- Credit
***
### Introduction

坂本千彰 SAKAMOTO Chiaki<br>

2016/3　　多摩美術大学美術学部情報デザイン学科 卒業<br>
2017/3　　同大学院修士課程 修了<br>
2018/4　　多摩美術大学美術学部情報デザイン学科 副手として勤務<br>

デザイン支援のためのジェネレーター開発を研究中<br>
[vimeo.com/chiaki82k](https://vimeo.com/chiaki82k)
***
### About Software
<img width="1080" alt="main" src="https://user-images.githubusercontent.com/22903046/48116550-cd820200-e2a9-11e8-97c3-9aae107312ff.png">

fff -HPShelfは,2017年7月に坂本千彰が制作協力した遊具を元に開発した**デザインファミリー**を生成するためのアプリケーションです.

![00](https://user-images.githubusercontent.com/22903046/48116033-2486d780-e2a8-11e8-8392-87d52cc4169c.jpg)

![01](https://user-images.githubusercontent.com/22903046/48116070-42543c80-e2a8-11e8-9022-7d91a0ff5cd8.jpg)
*木製HPシェル構造の子供用遊具（設計:小野田裕士、制作:坂本千彰、サトウフミタカ）*

ベースとなる棚形状から棚の幅,高さ,四隅の奥行きを設定することで,任意のサイズの棚をデザインすることができます.<br>
四隅の奥行きをそれぞれ違う値に設定することで,棚板,間仕切りがそれに伴って追従し,側面から見た形状が直線によって構成された曲面を描く, **放物双曲面**([hyperbolic paraboloid](https://goo.gl/s76R3r))が出来上がります.
<br>
<br>
<img width="1080" alt="03" src="https://user-images.githubusercontent.com/22903046/48117243-ee4b5700-e2ab-11e8-9fc2-603ef132b6b4.png"><br>
作成されたデザインは3Dデータ(PLY Format)と2Dデータ(Adobe Illustrator Format)として保存され,各種ファブリケーションツールを用いてプリントすることができます.
<br>
<br>
<img width="1920" alt="03" src="https://user-images.githubusercontent.com/22903046/48142293-df869380-e2ef-11e8-82ef-06f6a7d8ca87.png"><br>
※展覧会時配布データでは3Dデータのみのverを配布し,2Dデータは別途専用ソフトウェアを開発して実制作時に調整しました.
<br>
<br>
本作品の目的は,利便性の高いデザインソフトウェアを開発することではなく,**あるデザイン(定数)に選択できる範囲をつけ変数化することにより,個人の利用にフォーマットされつつも,元となったデザインを失うことなく保持する,デザインファミリーを生成する**ジェネレータソフトウェアの開発および,手法の検証になります.

***
### Working Process
![02](https://user-images.githubusercontent.com/22903046/48137931-7e0df700-e2e6-11e8-9ce6-de18c6f33298.jpg)

2018年11月,[多摩美術大学アートテーク](https://www.tamabi.ac.jp/art-theque/)で行われる[Beyoond Materializing展](http://www.idd.tamabi.ac.jp/~kubotaa/bmv.jpg)にて,実施実験としてfff -HPShelfを使用した展示台制作を行いました。展示空間や展覧会コンセプトに合わせ本来の棚アプリケーションを一部改変し,展覧会作家の協力のもと収集した希望展示台デザインの実制作を行なっています.
<br>
なおこのgithubプロジェクトにおいても,展覧会時に配布したアプリケーションデータをアーカイブとしてダウンロードすることができます.
##### 制作プロセス<br>
1. 展示台としてソフトウェアをチューニング.
2. 出展作家にソフトウェアを配布,生成された希望展示台データおよび,parameter logデータを収集.
3. parameter logデータに基づき図面作成用ソフトウェアを使用しcut outデータ生成.
4. cut outデータに基づき展示台の実制作<br>

※実制作に関しては[Shopbot](https://goo.gl/QB8Yio)を使用したCNC切削を想定していましたが,展覧会スケジュールに合わせ,[パネルソー](https://goo.gl/yHcjFh)などの工作機械を使用しています.
***
### Development Environment
**fff -HPShelfForMac**
- MacBook Pro (15-inch, 2016)
- macOS High Sierra ver10.13.3<br>

**fff -HPShelfForWindows**
- Surface Pro
- Microsoft Windows ver1803<br>
***
### Download Generator<br>

- [fff -HPShelf](https://github.com/chiaki88k/fff-HPShelf/archive/c00.zip)<br>
<br>
<img width="1920" alt="04" src="https://user-images.githubusercontent.com/22903046/48149681-119ff180-e300-11e8-95a2-e8a5f03214de.png"><br>

- [Artist Created Data](https://github.com/chiaki88k/fff-HPShelf/raw/c00/ArtistCreatedData.zip)<br>

***
### Thinking Note<br>

- ディスプレイ上の2次元であるデータを,プリントする,実用性のある家具のようなモチーフまでプリントするという試み
- オーダーメイド,レディメイド,カスタマイズ,ジェネラティブ,セルフプリント(ここでは平面表現)
- スケール感の消失,3Dプリントの最大造形サイズによって小物置きにも,椅子にも,机にも,屋根にもなるということ
- 最大パターン数の決まっているカスタマイズ設計ツールとの違い
- デザイナーが変数によるデザインファミリーを納品する時代
- CADツールにおいてのパラメトリックモデリング,ダイレクトモデリングとの違い
- UI設計やwebデザインのようなユーザーの画面サイズに依存するレスポンシブデザインとユーザーの生活にフィッティングすべきである家具デザイン,空間デザイン
- 乱数ではなく変数であり,ユーザーの求める解が得られるようなデザインをいかにパラメーターを用いて正規分布させるか.

***
### Credit<br>

##### 木製HPシェル構造の子供用遊具
- 設計:[小野田裕士](http://www.mawari.jp/onoda/)
- 制作:坂本千彰、[サトウフミタカ](http://www.tamabi.ac.jp/pro/g_works/2017/id/s19/)<br>

##### fff -HPShelf
- ソフトウェア制作/デザイン:坂本千彰<br>

##### Beyoond Materializing展 展示台制作
- 石島響
- 臼井達也
- 坂本千彰
- [サトウフミタカ](http://www.tamabi.ac.jp/pro/g_works/2017/id/s19/)
- 平山夏帆
- 山口千晶<br>

##### Beyoond Materializing展 展示台データ提供
- Beyoond Materializing展 出展者の皆さま
