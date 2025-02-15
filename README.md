# デザインシステムの学習メモ

## カラー選定
- **プライマリーカラー**：サイト・アプリのブランドイメージを伝える色で、主要なボタンや強調部分、ヘッダーなどに用いる。背景色とのコントラスト比が4.5:1以上を維持できるカラーにする必要がある。なお、プライマリーカラーは複数あっても良い。ブランドイメージやコンセプト、ジャンルからあったものをカラーパレットから選ぶ。[デジタル庁デザインシステム　カラーパレット](https://design.digital.go.jp/foundations/color/color-palette/)
- **セカンダリーカラー**：プライマリーカラーの補完的な役割をする色。選択肢を提供するボタンや、機能や状態を表すものなどに使用。プライマリーカラーと同じ色相で、明度の高低で決める。背景色とのコントラスト比は3:1以上にする。
- **ターシャリーカラー**：セカンダリーカラーと反対の明度で作る。セカンダリーカラーが明るいなら、ターシャリーは暗い色に。逆も同様に。
- **バックグラウンドカラー**：基本は白やグレー。他には、同じ色相でプライマリー、セカンダリーのコントラスト比を考えて選定すると良い。
- **ニュートラルカラー**：黒やグレー、白色。主にテキストや境界線などに使われる色。コントラスト比を考えて、適当な色を使う。
- **ステートカラー**：デフォルト時、hover時、acttive時の状態を表す色。
- **アクセントカラー**：特定の要素（CTAボタンなど）に注意を引きたい色に用いる。ただし、アクセントカラーを利用し過ぎると、デザインの統一感が崩れるし、アクセントカラーは必ずしも使う必要はない。
- **セマンティックカラー**：意味や目的を割り当てられたカラー。よく使うのは、サクセス時の緑系、エラー時の赤系など。基本的に、それぞれ、色相を保ち（サクセスなら緑、エラーや重要な警告なら赤）、サイトのイメージに合わせて、彩度や明度を調整する。
参考文献
[デジタル庁デザインシステム](https://design.digital.go.jp/foundations/color/)

## ボタンについて
- ターゲット領域を44px×44px以上に。
- もし44px以上ない場合は、上下の余白でターゲット領域を確保。
- ボタンは基本を三種類。背景色が色付きのもの、外周とラベルが色付き、テキストボタン。
- プライマリーボタンは最も重要なアクションに使用。原則一画面に一つまで。
- セカンダリーは、プライマリー以外の選択肢がある場合に使用。原則最大1画面に3つまで。
- ターシャリー：フローやアクションの実行を中断、中止するようなキャンセル行為のために使用。原則一画面で一つ。
- ボタンの配置は、未来は右方向、過去は左方向という世界観がWebブラウザでは形成されているため、完了、投稿などの進める系のボタンは、右側に。キャンセルや中止といったタスクを進行させないボタンは左側にするのが、ユーザーのメンタルモデルとも整合が取れる。ただし、モバイルの場合は、削除ボタン系が一番下。
- ボタンは基本時には重要度の高いものを右に並べる。ただし、PCでは慣習上、削除ボタンは左側に配置することが一般的だから左に配置している。ただし、ユーザーの認知の順序としては、
1. 選択肢（セカンダリー）の確認
2. 投稿するか判断
3. 投稿しないなら削除するかを検討
という順序になっている。だから、SPで縦配置の場合は、投稿ボタンの下に、削除ボタンが来る。

- ボタンのdisableはなぜ押せないのか明示する。
- ボタンの重要度を色の違いのにで表現しない。つまり似た色のセカンダリーカラーをセカンダリーボタンにすると、ロービジョンの人とかは判断しづらい。（察しの悪い人も理解しづらい。）ので、色だけでなく、形状で違いをつける。
- buttonもpointerに。

### 反省点
- セカンダリボタンを色違いで使ってた。
- 配置に関して、そこまで重要になるデザインやってなかったけど、わかってなかった。

- 参考文献
[デジタル庁デザインシステム　ボタン概要](https://design.digital.go.jp/components/button/)

