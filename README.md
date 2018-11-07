### **fff - HPShelf**
***
- Introduction
- About software
- Working process
- Requirements
- Download Generator
- Copyright
***
#### Introduction

坂本千彰 SAKAMOTO Chiaki
2016/3　 多摩美術大学美術学部情報デザイン学科 卒業
2017/3　 同大学院修士課程 修了
2018/4~  多摩美術大学美術学部情報デザイン学科 副手として勤務

デザイン支援のためのジェネレーター開発を研究中
[vimeo](https://vimeo.com/chiaki82k)
***
##### About software
<img width="1080" alt="main" src="https://user-images.githubusercontent.com/22903046/48116550-cd820200-e2a9-11e8-97c3-9aae107312ff.png">

このジェネレーターソフトウェアは、2017年7月に坂本千彰が制作協力した遊具を元に開発した**デザインファミリー**を生成するためのアプリケーションです。

![00](https://user-images.githubusercontent.com/22903046/48116033-2486d780-e2a8-11e8-8392-87d52cc4169c.jpg)

![01](https://user-images.githubusercontent.com/22903046/48116070-42543c80-e2a8-11e8-9022-7d91a0ff5cd8.jpg)
*木製HPシェル構造の子供用遊具（設計:小野田裕士、制作:坂本ちあき、サトウフミタカ）*

ベースとなる棚形状から棚の幅,高さ,四隅の奥行きを設定することで,任意のサイズの棚をデザインすることができます.
四隅の奥行きをそれぞれ違う値に設定することで,棚板,間仕切りがそれに伴って追従し,側面から見た形状が直線によって構成された曲面を描く, **放物双曲面**が出来上がります.

<img width="1080" alt="03" src="https://user-images.githubusercontent.com/22903046/48117243-ee4b5700-e2ab-11e8-9fc2-603ef132b6b4.png">

今回はBeyond Materializing展に合わせ本来の棚アプリケーションを一部改変し,展覧会作家の協力のもと,希望展示台デザインをそれぞれ作成していただき,実際の展示台の制作までを行なっています.

本作品の目的は,便利なデザインソフトウェアを開発することではなく,**あるデザイン(定数)に選択できる範囲をつけ変数化することにより,個人の利用にフォーマットされつつも,元となったデザインを失うことなく保持する趣旨の,言わばデザインファミリーを生成する**ジェネレータソフトウェアの開発および,手法の検証になります.

***
##### Working process
