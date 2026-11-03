# shopee-images

Shopeeマスアップロード用の商品画像ホスティング専用リポジトリ(public)。

各画像はJANコードをファイル名として保存しており、Shopeeマスアップロードの
Image URL列 (`raw.githubusercontent.com` 経由) から直接参照する。

- フォルダはジャンル別(`bodycare/` `cosme/` `haircare/` `makeup/` `menscare/`)。
- **出品している商品の画像だけを置く**(2026-10-07、82件)。出品しない・保留中の商品の画像は削除した。
  加工済みの元画像は非公開リポジトリ側のローカル `3_listings/<ジャンル>/framed/` に残っており、
  このリポジトリのGit履歴からも復元できる。
- 本体のリサーチ/出品ロジックは非公開リポジトリ `168cm63kg/shopee` で管理。

## extra/(追加画像、2026-11-04)

出品後の追加画像(英語・Canva作成)。`extra/<JAN>/cover.jpg`(枠付き表紙)と `1.jpg`〜`5.jpg`(①〜⑤)。
メディア一括更新(mass_update_media_info)の Cover image / Item Image 列から参照する。
