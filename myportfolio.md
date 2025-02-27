# Haato Watanabe（渡辺 羽亜人）

## About
所属：東京大学大学院 情報理工学系研究科 創造情報学専攻 梅谷研究室 修士　<br>
専門：コンピュータ・グラフィックス、特にコンテンツ制作支援とシミュレーションに興味があり、現在は3D Reconstructionの研究をしています。

- [Github](https://github.com/haato-w "Haato Watanabe Github home")
- [Wantedly](https://www.wantedly.com/id/haato_watanabe "Haato Watanabe Wantedly home")

<!-- -------------------------------------------------------- -->
***

## Publications
<!-- <dl>
  <dt>Comming Soon.</dt>
</dl> -->

<!-- <dl>
  <dt>Comming Soon.</dt>
</dl> -->

**Comming Soon.**

**Exploring User’s Line of Sight And Word Gesture Text Entry Techniques in Virtual Reality**
- Haato Watanabe, Ryo Hatano, Hiroyuki Nishiyama<br>
- Proceedings of the Joint Symposium of The Twenty-Ninth International Symposium on Artificial Life and Robotics (AROB 29th 2024)<br>
- VR空間において、目線で英字キーボード入力を行うシステムの提案、評価を行いました。

<!-- -------------------------------------------------------- -->
***

## Experience
**株式会社Preferred Networks**

<img src="imgs/PFN_logo.png" width="100px"/>

- R&Dサマーインターン、パートタイムエンジニア
- 4D Gaussian splatting web viewerの開発をしました。<a href="https://tech.preferred.jp/ja/blog/4d-gaussian-splatting-web-viewer/" target="_blank">成果ブログ</a>を公開しています。

**株式会社松尾研究所**

<img src="imgs/matsuo_logo.jpeg" width="100px"/>

- エンジニア インターン
- LLMを用いた業務効率化システムの共同研究プロジェクトに参加しました。

**株式会社プレイド**

<img src="imgs/plaid_logo.png" width="100px"/>

- エンジニア インターン
- webプロダクトの開発に参加していました。バックエンド、フロントエンド両方の開発を担当していました。
- キーワード：TypeScript, Express, Vue, Mongo, circleci, e2e, svelte, CDN

**株式会社Alice**
- エンジニア（業務委託）
- Edge AIの画像認識システムを開発をしました。既存プロダクトの調査、既存技術のサーベイ・検証、論文実装、システム設計、コーディングを一貫して個人プロジェクトとして行いました。
- キーワード：Keras, Tensorflow, ONNX, TensorRT, Jupyter, Git, Docker, Linux

<!-- -------------------------------------------------------- -->
***

## Works

**Making Visual hull mesh from mask images and camera params**

<video src="https://github.com/user-attachments/assets/37b00ca7-bea7-425f-9018-5901d05bca99" controls="true" loop="true" autoplay="true" muted width="600"></video>
<!-- https://github.com/user-attachments/assets/37b00ca7-bea7-425f-9018-5901d05bca99 -->
<!-- https://github.com/user-attachments/assets/c5bd42dd-4f6a-47c8-a2f9-fd9c84778653 -->

- 多視点画像データのカメラパラメータとマスク画像から対象物体のvisual hull meshを生成するコードを実装しました。
- visual hullを作成するコードは存在していたのですが、使いにくかったのでシンプルな仕様で作り直しました。
- 実装を公開しています。

**Nerf synthetic data creation code using Mitsuba renderer**

<img src="imgs/mitsuba_yuksel_hair_curly.png" width="400px"/>

- Mitsuba rendererを使用してNeRFのsyntheticデータを撮影する環境を作成しました。
- 公式実装ではBlender上のスクリプトで作成されていますが、Mitsuba rendererでデータを撮りたくなったので作成しました。
- 写真は[Yuksel hair dataset](http://www.cemyuksel.com/research/hairmodels/ "cem yuksel"){:target="_blank"}(curly)をレンダリングした例です。
- Mitsuba上でオブジェクトを配置してランダムな位置から撮影できます。
- ランダムに位置を決める処理や出力されるカメラパラメータファイルはNerf-syntheticデータセットを作成するコードに合わせて作っているので、3D Reconstructionに使いやすいと思います。
- コードに書かれている[jsonデータを設定することでレンダリングするシーンを変更](https://mitsuba.readthedocs.io/en/stable/src/generated/plugins_shapes.html "mitsuba document"){:target="_blank"}できます。
- 実装を公開しています。

**Stable fluids implementation**

<video src="https://github.com/user-attachments/assets/a12588de-e853-421a-a99f-04d1af530765" controls="true" loop="true" autoplay="true" muted width="300"></video>
<!-- https://github.com/user-attachments/assets/a12588de-e853-421a-a99f-04d1af530765 -->

- 流体シミュレーションの1種であるStable fluidsをCで実装しました。OpenMPを用いてSIMD並列化とスレッド並列化を行いました。
- Poisson方程式はJacobi法で計算しています。
- 元々流体シミューレーションに興味があったのでキャッチアップの最初のステップとして丁度良いと思い始めました。
- 書籍「GPU Gems」の38章「GPU上での高速な流体力学シミュレーション」が分かりやすかったです。


<!-- **3D Gabor Splatting** -->


**Gabor noise rasterizer in image space using pytorch**

<img src="imgs/gabor_noise_figure.png" width="500px"/>

<video src="https://github.com/user-attachments/assets/4e99b9c3-1890-4923-9db4-4c855d93b0ab" controls="true" loop="true" autoplay="true" muted width="500"></video>
<!-- https://github.com/user-attachments/assets/4e99b9c3-1890-4923-9db4-4c855d93b0ab -->
<!-- https://github.com/user-attachments/assets/0eeefd1f-b22f-45c2-ab16-bc9c953ce50c -->

- 画像空間でGabor noiseを生成できるコードです。
- pytorchで実装しているためexample imageに対してfittingをすることができます。
- 実装を公開しています。

**4D Gaussian Splatting Web Viewer**

<!-- <iframe width="560" height="315" src="https://www.youtube.com/embed/dPzrhA_5MDw?si=KoVLpvjnd7yvuY5a" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe> -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/uEdum66-xPc?si=eAeCWp-txWZRwIPq" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

- プリファード・ネットワークスのR&Dサマーインターン、アルバイトで動きのある3D Sceneを再構成する手法である4D Gaussian SplattingのWeb Viewerを開発しました。PCとモバイルデバイスの両方で動作します。
- WebGLとReactで開発を行いました。シェーダーでのレンダリング処理やカメラ操作、視点変更UIのための衝突判定処理等を実装しました。
- ウェブブラウザという限られた環境の中で様々な処理を行う必要があるため、処理の効率化やスレッド並列化を特に工夫しました。
- サマーインターンにおける開発成果は[**テックブログ**](https://tech.preferred.jp/ja/blog/4d-gaussian-splatting-web-viewer/ "PFN Tech Blog"){:target="_blank"}として公開しています。
- 時間周りは書籍「ゲームエンジン・アーキテクチャ」の7.4, 7.5章の時間の扱いが参考になりました。

**C Standard Library reimplementation**
- 低レイヤのコードに慣れようと思い、C標準ライブラリを再実装しました。
- 実装難易度は全く高くないですが、自分で書くと細かい仕様を学べるので楽しかったです。
- [**実装を公開しています。**](https://github.com/haato-w/my-c-standard-library "github repository"){:target="_blank"}

**視線によるキーボード入力アプリ**

<div align="center">
<img src="imgs/eye_gesture_playing_situation.png" width="400px"/>
<video src="https://github.com/user-attachments/assets/b8325822-dc42-422c-8833-4242fbcbc9ca" controls="true" loop="true" autoplay="true" muted width="400"></video>
</div>
<!-- https://github.com/user-attachments/assets/b8325822-dc42-422c-8833-4242fbcbc9ca -->

- Meta Quest上でどうさする視線で英字キーボードを操作できるシステムです。
- 視線でキーボードをなぞり、ジェスチャータイピングを行うことで英単語を入力できます。
- 動画は与えられたテキストを視線で入力している様子です。
- マウス操作は目で行い、選択はコントローラで行います。
- [**実装を公開しています。**](https://github.com/haato-w/VRKeyBoardUsingGestureTypingWithEyeTracking "github repository"){:target="_blank"}

**ペリペリ感触アプリ**

<video src="https://github.com/user-attachments/assets/f83fb95f-f8f6-4a55-b9c2-7871669fbf96" controls="true" loop="true" autoplay="true" muted width="400"></video>
<!-- https://github.com/user-attachments/assets/f83fb95f-f8f6-4a55-b9c2-7871669fbf96 -->

- iOS上で動作する「くじ引きをめくっているときのペリペリ感を体感する」ことができるアプリを開発しました。スマホの画面を指でなぞるとくじがめくられるアニメーションが動作し、バイブレーションによりくじをめくっている感触を体験できます。
- ハイカジュゲームを作る過程で実験のために作りました。
- 動画はめくっている様子を示しています。めくる動作と同時にバイブレーションでぺりぺり感を演出します。
- アニメーションはUnity、バイブレーションはCore Hapticsを用いて開発しました。
- Test Flightで配布してテストしていました。

**Ray-tracing implementation**

<img src="imgs/render_12000.bmp" width="100px"/>

- 趣味でRay-tracingをC++で実装しました。
- 画像はコーネルボックスの100x100pxでレンダリングした結果です。

**ナンバープレート認識システム**
- Edge AIコンピュータのJetson Nano上で動作する日本語ナンバープレート認識システムを開発しました。
- 研究開発案件で開発しました。
- 開発当時、Nvidiaが公開しているLPRモデルが日本のナンバープレートに対応していなかったため、日本のナンバープレートに対応するシステムを開発しました。
- プロジェクトの過程で作成したコードを公開しています。tensorrt infer、google-drive-docment-ocr、deepstream_lpr_app_python、ImageDataAugmentation

**姿勢監視タスク管理アプリ**

**DeNAハッカソンのサイト**

**android code learning app code**

<!-- -------------------------------------------------------- -->
***

## Awards
- 2022 DeNA オータムハッカソン 優勝

<!-- -------------------------------------------------------- -->
***

## Misc.
- TOEFL iBT: 79 (2022 September)
- TOEIC L&R: 920 (2023 February)
- 応用情報技術者試験
- 42 Tokyoに所属しており、低レイヤ側の開発の練習をしています。
