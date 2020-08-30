---
author: ameblo
title: "\n\t\t\t\tNV_transform_feedback\t\t"
slug: nv_transform_feedback
id: 3356
date: '2007-09-04 02:01:38'
layout: post
categories:
  - Graphics
---

masafumiくんのBlogでD3D10の「Stream output」をOpenGLでどうやって実装するの、という話があって、その流れで見つかったIcare3dのフランス語ページ。

[http://developer.download.nvidia.com/opengl/specs/GL_NV_transform_feedback.txt](http://developer.download.nvidia.com/opengl/specs/GL_NV_transform_feedback.txt)

[http://www.icare3d.org/content/view/48/9/lang,fr/](http://www.icare3d.org/content/view/48/9/lang,fr/)

**<span>Transform Feedback.</span>**

<span>(_NV_transform_feedback_)</span>

<span> </span>

<span>Il s’agit de l’implémentation OpenGL de la fonction de stream output de DirectX 10\. Elle permet de récupérer (dans un buffer object) les attributs de sommets générés par le vertex shader ou le geometry shader plutôt que ceux-ci soient envoyés pour assemblage et rasterisation. Elle permet ainsi de désactiver l’étape de rasterisation du pipeline. Les données une fois dans un buffer object peuvent être réutilisés comme vertex buffer, pixel buffer, texture buffer ou parameter buffer object (cf. plus loin).</span>

<span></span>

<span>とりあえず訳してみる。</span>

<span></span>

<span>Transform　Feedback　(NV_transform_feedback)はDX10のStream outputのOpenGLにおける実装として機能します。これは(バッファオブジェクト内で)アセンブラとラスタライゼーションに送られたジオメトリシェーダもしくは頂点シェーダによって生成されたアトリビュートのサマリーを取得します。 この機能はパイプラインのラスタライズステージを不可することを許可し、データは頂点バッファやピクセルバッファ、テクスチャーバッファやパラメータバッファオブジェクトのように、ひとつののバッファオブジェクト内で1回、再利用可能です(将来実装)。</span>

<span></span>

<span>多分これぐらいのフランス語なら訳せる…間違ってないと思うけど。</span>

<span>それにしてもGPUVision的な使い方（といってもこいつはPSが多いけど）とかに限らず、ジオメトリシェーダなどを利用したGPGPU利用だと、必ず出てきそうな話題だけど、意外と情報がないのね。</span>

<span></span>

<span>以上、とつぜんCGの話題でした。</span>

<span></span>

<span></span>