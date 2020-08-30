---
author: ameblo
title: "\n\t\t\t\tVirtools User day @ Ingenierium\t\t"
slug: virtools-user-day-ingenierium
id: 3019
date: '2006-09-20 01:50:38'
layout: post
categories:
  - '[Re]virtual reality'
tags:
  - Server
---

<div>以下、本当に会議参加メモ。未編集。 フランス語わからん人はぜんぜんわけわからんと思うので、興味あるひとは質問してくださいな。</div>

<div>あと、一部wiki表記なので、このエントリーに関しては、こっちのほうがいいかもしれないです。</div>

<div>[http://akihiko.shirai.as/modules/bwiki/index.php?Blog%2F2006-09-19](http://akihiko.shirai.as/modules/bwiki/index.php?Blog%2F2006-09-19)</div>

<div>---- 研究所の核であるCLARTEによる主催で、産業用CADで有名なDassault Systemグループになった「Virtools」のユーザ会が開催された。 [http://www.clarte.asso.fr/](http://www.clarte.asso.fr/)</div>

<div>せっかくの地元開催なので、自分たちの研究室のデモブースも準備。 昨年度の修士学生のプロジェクト6点のビデオと、学生プロジェクトである子供服店舗シミュレーター「VirtualKid」のリアルタイムデモを準備。</div>

<div>以下、午前のアジェンダ。</div>

<div>10h30 - 13h30 Retour d'Experiences --[Automobile] PSA PEUGEOT CITROEN  Thierry Vollequin  Acteur majeur de l'industrieautomobile europenne et mondiale.</div>

<div>--[Naval] DCN  Yves Le Therisien   Expert europeen et mondial des systems navals,</div>

<div>--[Patrimoine] Nautilus  Pascal Sultan   Specialiste en realite virtuelle et simulation.</div>

<div>--[Archeologie] UMR CNRS Univ. Bordeaux 3 Bruno Dutailly   Pole europeen specialiste dans les domaines des sciences de l'Antiquite, l'archeologie antique et medievale.</div>

<div>以下、プレゼンメモ。</div>

<div>PSA Peugeot Citroen</div>

<div>VR研究センターについて オートステレオ、CAVEなどなどもあるが 以下具体的事例紹介</div>

<div>ユーザオペレーション評価 上半身モデルと両手に持ったIRポインタで操作。 車の後部ハッチの開閉や荷物の積み入れなど、視界も評価</div>

<div>操縦席シミュレーション、物理的なモックアップを使用</div>

<div>Metier Peinture 塗装技術演習 自動機械で塗れない細かい点の塗装に関する技術習得用VR</div>

<div>Metier Montage</div>

<div>Amenagement  du poste de travail TOYOTAとの共同開発？ バーチャル工場における作業シュミレーション 上記、オペレーション評価と同じく上半身モデルでバーチャル組み立て評価。 以下ビデオに写っているパラメータについて考察。 -Hauteur Main…おそらく腕の高さ(m)。高いほどつらい、無理な姿勢。 -Distance Parcourue…作業間距離、長いほど無駄な歩きが多くなる -Mode Agence…なんだろう？</div>

<div>-Fonctionnalites utilisees --Import d'important flux de donnes CAO --Scenarisation --Navigation --Animation --Detection de Collision --Haut neveau d'interactive --Export</div>

<div>-Capitalisation des methodologies --Modules regroupant des fonctionnalites dediees --a la gestion des systemes --a la creation d'interactions</div>

<div>-Intergration des scenarii dans une scene de base unique, construite sur les modules -Creation cration de modules Metiers --Protocoles d'evaluation de prestations --Avatar --Simulation d'operations Process</div>

<div>Forces et faiblesses Virtools 使用上の評価いろんな点についてよい、普通、など… -Import/Export まあまあ -Gestion de la scene 良い (メモしきれなかったが7項目ぐらい) -etc...</div>

<div>Meilleure integration CAO /Realite Virtuelle 上記各事例、Mayaとの連携、ワークフローなど含め、 CAD、Preparation、Scenarisationなどで出口を、Conception Produit, Conception Processとして よりよい活用の仕方をまとめていた。</div>

<div>Amelioration de la qualite de rendu フォトリアリスティックなプリレンダー画像(で観衆を圧倒させてみる、すごい)</div>

<div>-Perspectives --Conception en environnement immersif --Immersion et interaction multi modales --Collaboration entre humain et avatar(s)</div>

<div>---- [Naval] La Realite Virtuelle a DCN   Yves Le Therisien</div>

<div>冒頭に軍事関係のVRデモビデオ。CAVE内で軍用艦(特に空母)のデザインと評価。 内装関係、オペレーションデスクなどをIRポインタで配置し、見え方を評価したり、長さを図ったりできる。 軍事関係でなくても家の内装でも使えそう。</div>

<div>デジタルモックアップに必要となる話をいくつか (正直なところあまり面白くない)</div>

<div>-De par sa vocation, DCN assure... -Les critere lies a l'emmenagement --La realite virtualle permet la prise en compte et la verification de... -Une application sous Virtools --DCN dans le cadre de son partenariat avec CLARTE a fait developper un demonstrateur d'application d'emmenagement sur Virtools: ---Portable sur espace hautement immersif type SAS3 ---Avec un haut nivbeau de realisme ---Adaptable a differents formats d'entree CAO ---Permettant l'evaluation des criteres --Cette application a ete evalueee par un panel d'utilisateurs</div>

<div>(プレゼンテーター交代、若いエンジニア、見たことある、多分CLARTEの人)</div>

<div>Objectif: Developper une application permettan la validation de l'amenagement d'un local en utlisant la realite virtuelle. #1 Menu: Les fonctionnalites de l'application sont accesibles grace a un menu 3D de type "command & contorl cube" ファンクションに対応する2D絵の描いてあるパネルを使って操作を補足する。例のELディスプレイとか使えばよりよさそう。 #2 Analyse Visuelle: L'utilisation du tracking en envbironment immersif permit une analyse temps reel des zones de visbilite sur la maquette numerique. Cela permet aussi la perveption des volumes de la maquette pour evaluer des ecombrements, des accesibles, etc... #3 Emmenagement: L'utilisateur dispose d'outils lui permettant d'evaluer un amenagement extistant. #4 Mesure de distance: L'utilsateur dispose d'un outil lui permettant de mesurer des distances. #5 Mesure d'angle: #6 Ergonomie: l'utilisateur dispose d'unhumain virtuel dontrolable en cinematique inverse. 　Maxのキャラクタースタジオに近い骨格。衝突などを評価。</div>

<div>(感想)軍事関係だけにコメントしづらい部分もあるし、プレゼン自体が堅いのだけど、空母の内装、操縦桿の設計などは、実際、図面よりもVRで評価したほうが全体残すとダウンと性能にはつながるよな…と理解しておくことにする。日本だったら建築関係の事前評価(施主さんがユーザ)に非常にマッチすると思う。</div>

<div>----- [Patrimoine] Nautilus  Pascal Sultan 人数構成、事業所面積、など概要。</div>

<div>-Secteurs d'activites; --Industrie --Partmoine --Ludo-Pedagogique</div>

<div>(プレゼンテータ交代)</div>

<div>-VirtoolsユーザとしてのNautilus 2002年のVirtools Dev2.5より使用 -Demande de Nautilus 要求事項 --Forte Qualite Graphique --Stereoscopie --Clustering --Moteur permettant de gerer...</div>

<div>-Nos + du Moteur Virtools Dev: -- Integration de nos propres Shaders -Le VRPack (Stereo, Clustering) -Moteur Oriente Dvpt: Facilite d"integration de nos systems d'operation -etc</div>

<div>このへんVirtools Webplayerをつかったシェーダーデモなどを混ぜる…かっこいい！ -石像のLODデモ -エリゼ宮？のスクリーンショット。超ハイポリゴン</div>

<div>-Nos - du moteur Virtools Dev: --Prenne du retard en terme de qualite de rendu (MipMapping, Antialiasing,etc) --Expoteur en dessous des capacitees du moteur (necessite un retraitment) --etc</div>

<div>Conlusion -Pour les grosses scenes, Virtools est interessant --Cote Oriente Developpement compense le cout des licenses. --Un bon workFlow compense le rendu graphique (DDS, NormalMap, etc...) --etc</div>

<div>(プレゼンテータ交代) Ludo Educatif et Industriel エデュテイメント、企業応用</div>

<div>-Nos Besoins 我々の要求事項 --Bon niveau Visuel --Facilite fe development --Clustering (=multiplayer) --SDK ouvert</div>

<div>-Nos + du moteur Virtools Dev: --Interfacage de nos peripheriques simplifies --Multi-scran simplifie --Moteur Oriente development, prototypage raipde d'agents intelligents, de qqch...</div>

<div>-Nos -Moins du moteur Dev: --Le cout des licenses VRPack...pour un cluster  クラスターで使うVRパックのライセンス料 --Organisation du VRPack (Fichier texte, repertoire, gestion license, etc...)　</div>

<div>-Photo --農耕機械のシミュレータ --Madrace(実際の車の廃車をつかったマルチプレイヤーレースゲームシステム) --Virtual Sulky(一人乗り二輪馬車のレースゲーム、馬車と綱の部分が実物)</div>

<div>-Conclusion --Virtools est un tres bon moteur quand le cote developpment de l'appliucation predomine face au cote graphique (integration peripheriques (gant trackers, IA,etc))</div>

<div>----- [Archeologie] UMR CNRS Univ. Bordeaux 3 Bruno Dutailly Presentation d'Ausonius et de la plateforme techonogique 3d du CNRS.</div>

<div>-Methods --Modelisation ---PDMS/Review depuis les annee 80 --3DSMax --Discussions ---Seminairres avec les specialistes ---Production de modeles 3D valides scientifquement</div>

<div>-Outils --Salle de modelisation et developpement --Salle de realite virtuelle polyvalente ---Seminaires ---Presentation au public --Cluster de PC --Stereo --Virtools</div>

<div>-Video VRシアター、セミナー用、200席ぐらいあるか？後部が高くなる円形闘技場方式、4プロジェクタでステレオ表示可能。 どうやら横方向に2画面つないでいるようだ。 --デモ1は遺跡関係の発掘物。Virtoolsで表示。2004年に見たことあるかも。 --デモ2は遺跡の復元と思われる。古代の水道？ --デモ3は階段状の祭壇？こんなシアターでこの手の建築物をステレオで見るのって変な気分だろうな。柱の細部などはたくさんポリゴンを割いてモデリングしている。マテリアルはついてない。</div>

<div>-Virtools --Gestion du cluster --Gestion de la stereo --Dendus pilyvbalents: OpenGL ou DirectX --etc</div>

<div>-Demo: Les Maidum Bowls --Web Playerをつかったデモ --古代の土器をWeb3Dで見れるようにしている</div>

<div>-Demo: Budda --高密度3Dスキャンによる仏像顔面をWeb Playerでデモ</div>

<div>----</div>

<div>昼食をはさんで自分たちのデモがあって15時からVirtoolsのデモ</div>

<div>----</div>

<div>David (デモがあったので途中から参加)</div>

<div>-Virtools workflow for product experience --Design (PLM) --Import --Dreate ---Experience すべてのプロセスをDassaultの3D XMLで通す。</div>

<div>-Virtools 4 Product Line --Capture (Import) --Give Life (create) Virtools 4 --DEPLOY/EXPERIENCE (Publish)  PC Exe, Mac Exe, Xbox Exe, Office/CD/ SKU... Interenet, Intranets/ immersive</div>

<div>-Virtools VR  History --Behaviors 3D Visu / Dev1.0 1999 --Virst VR device Addons / Dev2.0 2000 --VR Cluster sand VRDevices in VRPack ...</div>

<div>-Some industrial VR References 松下のディスプレイは大きく扱われているなあ…</div>

<div>-Some VR Hardware partners --BARCO, HP , Ascension, ORAD, HAPTION, nVIDIA, etc...</div>

<div>-VR Technical Architecture View --VR Core (VRK) --Hareware Config --Remote ctrl --SDK Access to other features --VR  Visu (VRV) ---Stereo ---VR Camerea(asymmetrical) ---Multi-view ---Wrapping /Blending VR managers {generic edge blending, elumens} ---VR Cluster (VRC) ---Sync --etc(書ききれなかった...)</div>

<div>-Vrtools VR Library</div>

<div>-VR Publisher --Hardware portablity ---Transparent interchange of VR experiences between different VR centers and displays --Configration scalability ---Multi head ---Multi GPU/ CPU ---Cluster --Remote control and logging ---Cluster becomes a commodity --Device server --Calibration tools ---Takes minutes, not hours --Scalable offer ---Per player pricing ---Per hardware level pricing (L1,L2,L3)</div>

<div>-Decated offers per Hardware class --L1: Fish tank VR, HMD, Simple projection, Stereo Projection pair --L2: Medium walls, small clusters, flat only walls --L3: Large walls, Large clusters, CAVE , domes, RC (松下のディスプレイなど)</div>

<div>Expected deployment による</div>

<div>[What's new in Virtools 4] -Summary -Native support for 3D XML --Exchange files from/to CATIA, ENOVIA, DELMIA., SoldWorks --Using authoring (Resourse >IMport/Export) --At tuntime (Object Load BB)</div>

<div>--Some limitations ---2D SVG Representations ---Lines ---Industry Specific Extensions (require CAA API for development ) ---Data without an equivalent in Virtools context</div>

<div>-3D XML Fundamentals 'Standard XML and Extendable Format グラフィックスプロパティとマテリアルの下層に暗号化バイナリーもサポートする</div>

<div>-Standards support OpenGL --Support of CGFX shaders for OpenGL in addition to HLSL shaders for DirectX --Support of OpenGL 2.0 extentions ---CGFX + OpenGL = HLSL+ DirectX COLLADA COLLADA is an open Digital Assert Exchange Schema for the media/entertainment 3D industry --Version supported by Virtools: Collada1.4 --Improve DCC asset workflow --Current Limitations ---No shader support ---Animation: Only baked transfortmation matrices</div>

<div>-Virtools Improvements --65536 vertices per mesh limit as been removed ---Opens Virtools platform to a wider range of users (particulaly CAD users) working with more high-def models --Save optimized mesh version --Joystick support improved ---Rescan devices at runtime ---Support of XInput joystick (Xbox360 joystick compatible) ---etc...</div>

<div>-Experieence: 3D For All, 3D Everyone -3D Life Player --Renamed (was Virtools Web Player) --Improve online installation process (rewrite HTML code) --New update system --Compatibile with Virtools Web Player 3.5 --MacIntel: in the pipe but no release date yet --New limitations: ---ActiveX check the host is really Internet Explorer ---Plug-in only load standard Virtools plug-ins プレゼンではFireFoxのアイコンがあるのだけど、FireFoxのadd-onsはサポートされるのかしら？</div>

<div>-3D Office / 3D XE Player 新しいWebプレイヤー (SIGGRAPHで見たがシナリオを組み込める) スタンダードマニュピュレーション環境になるらしい。 -Product + Context + Scenario = User Experience --Product ---3D objectsd (NMO, 3DXML) ---Parts assembly ---Intrinsic behaviors ---Metadata --Context ---3D Environment (NMO, 3DXML ) ---Background image (JPG, PNG, BMP, etc) no direct user interactions --Scenario ---User point of view (camera) ---Standard nabigations (NMO) ---Standard manipulations )NMO_ ---Activates ---etc</div>

<div>Aotobotive, Aerospace, AEC, CPT においてProduct/Context/Scenarioの例を紹介。</div>

<div>-Simplified clustering development --Dynamic Distribution</div>

<div>-Application templates for instant VR authoring (VRNR) --No need to be a Scripting expert to start using the VRPack ---User VRNav template as astarting point OR... ---SImply drag and drop a few scripts from the VRPack Normalized Resourse(VRNR) library. --Applications made with VRNR are 100% portable across any VR hardware configuration --VRNR sources are provided (although not supported) making an idea best practice sample framewrok to build your own.</div>

<div>-Stunning set of highly portable VR demos ((VRDKit1.0) --Showcase the potential of your new VR room before your own applications are ready --Enables you to validate that your hardware is properly setup ---Easy to setup on any hardware thanks to the VRNR --Only requires VRPack Publishing Edition --Features ---VRConfTest for calibrating your video and tracking equipment (おお！) ---VRPlane ---VRBoat (TBC) ---etc...</div>

<div>-What's next? -VRWithin PLM</div>

<div>-XE-VR VR to become standard "VR for All" --VR will become a "technology pack" for XE-based applications --Trageted to end-users, not developers, like XE --VR hardware will be standardized through a new XML description, like P C S, which aims to become a standard ---Trackers, Displays, Cluster --Ready to use Scenarios ---Generic</div>

<div>-Future technical tracks Game technology  will always drive VR --Multi-platform Virtools core and GUI --Multi-thread., multi-pipe --Muilitple OS --Remote authoring /debbuging for cluster --Support for VR game decicess (eg. PS3 and Wii)</div>

<div>そのあと、カクテルになる。 VirtoolsのDavidがお疲れ＆懇談にお忙しいところを引っ張り出して、自室でVideoPlayerデモを解説してもらう。 簡単に言えば、ATIのVideoShaderデモに近いことが用意されているサンプル。ソースはVideoFile、Live(カメラね)、Streamが選べる。 ふむふむ、なるほど、これは動くなあ…。BBはその名も「VideoPlayer」。 以前別のサンプルを試したときはカメラの初期化でこけたんだけどなあ…やはり開発側の人間がいると話が早い(というかこのデモは難なく動いた)。</div>

<div>GPUVisionをここで実装したらいいじゃん、という提案をされる(Simonも)。 でもHLSLのソースコードをPublicにするのはどうかと思うんだけど…と難色してみたら、 実はスクリプトの書き出しオプションでDev上で見れなくすることができるらしい。なるほどこれで可能だなあ。 新しいVirtools4でのカメラプロパティ操作も良くなるらしいし(サポート列挙を作ってから選択する形式)、コードの圧縮暗号化もサポートするとのことで、状況整いすぎだなあ…。 うむむ。</div>

<div>写真とかスクリーンショットはそのうち上げようと思うがとりあえず何かみたい人はここがいいかも。 [http://www.virtools.com/News/events/event_laval_06.asp](http://www.virtools.com/News/events/event_laval_06.asp)</div>