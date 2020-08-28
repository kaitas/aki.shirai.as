---
author: ameblo
title: "\n\t\t\t\tPapers/Appearance Capture &amp; Editing\t\t"
slug: papersappearance-capture-amp-editing
id: 3326
date: '2007-08-09 02:14:05'
layout: post
categories:
  - SIGGRAPH
---

<div align="center">[![S5031316.JPG](http://blog-imgs-42.fc2.com/a/k/i/akihikofr/blog_import_4f5649b55fcaa.jpg)](http://blog-imgs-42.fc2.com/a/k/i/akihikofr/blog_import_4f5649b57c349.jpg)</div>

どれも面白そうな発表だったんだけど、朝もたもたしてたので中盤から聴講。 **Multiscale Shape and Detail Enhancement From Multi-Light Image Collections** A new method to enhance detail and surface shading using a few images with different lighting. Our approach uses a new, fast multi-scale bilateral image decomposition. Raanan Fattal, Maneesh Agrawala (University of California, Berkeley)

Szymon Rusinkiewicz (Princeton University) **Post-Production Facial Performance Relighting Using Reflectance Transfer** Facial performance video relighting using quotient images and optical flow to transfer reflectance from a static reflectance field to the performance, showing both same-subject and cross-subject cases. Pieter Peers (USC Institute for Creative Technologies) Naoki Tamura (The University of Tokyo and Mitsubishi Electric Research Laboratories (MERL)) Wojciech Matusik (Mitsubishi Electric Research Laboratories (MERL)) Paul Debevec (USC Institute for Creative Technologies) （これ見たかったんだけど、間に合わなかった） **Interactive Editing and Modeling of Bidirectional Texture Functions** A new approach for interactively manipulating and creating bidirectional texture functions. Jan Kautz (University College London) Solomon Boulos (University of Utah) Fre'do Durand (Massachusetts Institute of Technology, Computer Science and Artificial Intelligence Laboratory) BTFを操作する、という研究。 BTFをオリジナルから光線空間において、Blur/Shapenさせることによって表面の質感を変える、 毛糸の編み物のようなテクスチャについて、正面ライトと側面ライトで撮影した2つの除算で影エリアを算出し、影除去を行う、パララックスをレタッチするなど。 「BTFShop」なるツールを開発。 **AppWand: Editing Measured Materials Using Appearance-Driven Optimization** A stroke-based approach to editing spatially and time-varying measured reflectance that smoothly propagates user-supplied editing constraints using an appearance-driven optimization. Fabio Pellacini (Dartmouth College) Jason Lawrence (University of Virginia) [http://portal.acm.org/citation.cfm?id=1276377.1276444&coll=portal&dl=ACM&CFID=15151515&CFTOKEN=6184618](http://portal.acm.org/citation.cfm?id=1276377.1276444&coll=portal&dl=ACM&CFID=15151515&CFTOKEN=6184618)

今度はBRDFを操作する、という研究。インタラクティブに。 ちなみにメタリックな反射なども含むマテリアル。 NPRスケッチみたいに、マウスで箇所を指定するだけで操作できる。 appearance graph→sparse embedding 結果のパートで、他の方式（Marschner, 2005）との比較を行う、という発表形式を行っていた。 デモの解像度は低いけど、本当にインタラクティブに操作できているのがいい感じ。 錆び、木目とかも制御している。 Lischinski,2006の方式と比べて、マスクの描き方が違う。 提案方式はエッジのハッキリしたマスクを生成するようだ。