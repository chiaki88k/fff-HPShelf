## **fff -HPShelf**
***
- Introduction
- About software
- Working process
- Development environment
- Download Generator
- Credit
***
### Introduction

坂本千彰 SAKAMOTO Chiaki<br>

2016/3　　多摩美術大学美術学部情報デザイン学科 卒業<br>
2017/3　　同大学院修士課程 修了<br>
2018/4　　多摩美術大学美術学部情報デザイン学科 副手として勤務<br>

デザイン支援のためのジェネレーター開発を研究中<br>
[vimeoLink](https://vimeo.com/chiaki82k)
***
### About software
<img width="1080" alt="main" src="https://user-images.githubusercontent.com/22903046/48116550-cd820200-e2a9-11e8-97c3-9aae107312ff.png">

fff -HPShelfは、2017年7月に坂本千彰が制作協力した遊具を元に開発した**デザインファミリー**を生成するためのアプリケーションです。

![00](https://user-images.githubusercontent.com/22903046/48116033-2486d780-e2a8-11e8-8392-87d52cc4169c.jpg)

![01](https://user-images.githubusercontent.com/22903046/48116070-42543c80-e2a8-11e8-9022-7d91a0ff5cd8.jpg)
*木製HPシェル構造の子供用遊具（設計:小野田裕士、制作:坂本千彰、サトウフミタカ）*

ベースとなる棚形状から棚の幅,高さ,四隅の奥行きを設定することで,任意のサイズの棚をデザインすることができます.
四隅の奥行きをそれぞれ違う値に設定することで,棚板,間仕切りがそれに伴って追従し,側面から見た形状が直線によって構成された曲面を描く, **放物双曲面**([hyperbolic paraboloid](https://goo.gl/s76R3r))が出来上がります.<br>


<img width="1080" alt="03" src="https://user-images.githubusercontent.com/22903046/48117243-ee4b5700-e2ab-11e8-9fc2-603ef132b6b4.png"><br>
作成されたデザインは3Dデータ(PLY Format)と2Dデータ(Adobe Illustrator Format)として保存され,各種ファブリケーションツールを用いてプリントすることができます.
<img width="1920" alt="03" src="https://user-images.githubusercontent.com/22903046/48142293-df869380-e2ef-11e8-82ef-06f6a7d8ca87.png"><br>
※展覧会時配布データでは3Dデータのみのverを配布し,2Dデータは別途専用ソフトウェアを開発して実制作時に調整しました。<br>
本作品の目的は,便利なデザインソフトウェアを開発することではなく,**あるデザイン(定数)に選択できる範囲をつけ変数化することにより,個人の利用にフォーマットされつつも,元となったデザインを失うことなく保持する趣旨の,言わばデザインファミリーを生成する**ジェネレータソフトウェアの開発および,手法の検証になります.

***
### Working process
![02](https://user-images.githubusercontent.com/22903046/48137931-7e0df700-e2e6-11e8-9ce6-de18c6f33298.jpg)

2018年11月,[多摩美術大学アートテーク](https://www.tamabi.ac.jp/art-theque/)で行われる[Beyoond Materializing展](http://www.idd.tamabi.ac.jp/~kubotaa/bmv.jpg)にて,実施実験としてfff -HPShelfを使用した展示台制作を行いました。展示空間や展覧会コンセプトに合わせ本来の棚アプリケーションを一部改変し,展覧会作家の協力のもと,希望展示台デザインをそれぞれ作成していただき,実際の展示台の制作までを行なっています.
<br>
なおこのgithubプロジェクトにおいても,展覧会時に配布したアプリケーションデータをアーカイブとしてダウンロードすることができます.
##### 制作プロセス<br>
1. 展示台としてソフトウェアをチューニング.
2. 出展作家にソフトウェアを配布,生成された希望展示台データおよび,parameter logデータを収集.
3. parameter logデータに基づき図面作成用ソフトウェアを使用しcut outデータ生成.
4. cut outデータに基づき展示台の実制作<br>

※展示台の実制作に関しては[Shopbot](https://goo.gl/QB8Yio)を使用したCNC切削を予定していたのですが,展覧会スケジュールに合わせ,[パネルソー](https://goo.gl/yHcjFh)などの工作機械を使用しています.
***
### Development environment
**fff -HPShelfForMac**
- MacBook Pro (15-inch, 2016)
- macOS High Sierra ver10.13.3<br>

**fff -HPShelfForWindows**
- Microsoft Windows ver1803
- Surface Pro<br>
***
### Download Generator<br>

- [fff -HPShelfForMac](https://github.com/chiaki88k/fff-HPShelf/raw/c00/HPShelfForMac.zip)<br>
- [fff -HPShelfForWindows](https://github.com/chiaki88k/fff-HPShelf/raw/c00/HPShelfForWindows.zip)<br>
- [Artist Created Data](https://github.com/chiaki88k/fff-HPShelf/raw/c00/ArtistCreatedData.zip)<br>

***
### Credit<br>

###### 木製HPシェル構造の子供用遊具
- 設計:小野田裕士
- 制作:坂本千彰、サトウフミタカ<br>

###### fff -HPShelf
- ソフトウェア制作/デザイン:坂本千彰<br>

###### 展示台制作
- 石島響
- 臼井達也
- 坂本千彰
- 佐藤史崇
- 平山夏帆
- 山口千晶<br>

###### 展示台制作協力
- Beyoond Materializing展 出展者の皆さま
