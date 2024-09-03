# land-volume-calc-site
標高タイル等から土地の体積を簡易的に試算するサイト

https://mghs15.github.io/land-volume-calc-site/

* 作図したポリゴン内にメッシュを発生させ、各メッシュの標高値等及び面積から体積を試算します。
* 標高タイルを用いた土量の他、湖沼深タイルを用いて湖の体積も試算できます。

精度はかなり大雑把なので参考程度にお願いします。また、試算時に表示される柱の高さは強調しています。

## 実験
* 西之島：約98,868,054立法メートル（約100 m メッシュ）
  * 公表値は[体積は9,992万 m<sup>3</sup>（2019年5月）](https://www8.cao.go.jp/okinawa/siryou/singikai/senmoniinkai/14/14-3-2_1.pdf)
* 摩周湖：約2,787,610,163立法メートル（約250 m メッシュ）
  * 公表値は[湖容積 28.6億 m<sup>3</sup>](https://db.cger.nies.go.jp/gem/inter/GEMS/mashu/contents/intro.html)

## 使用データ
### 体積計算用
* [標高タイル](https://maps.gsi.go.jp/development/ichiran.html#dem)
* [湖水深タイル](https://maps.gsi.go.jp/development/ichiran.html#lakedepth)

### 背景地図
* [最適化ベクトルタイル](https://github.com/gsi-cyberjapan/optimal_bvmap)
* ハザードマップポータルサイト [洪水浸水想定区域（想定最大規模）](https://disaportal.gsi.go.jp/hazardmapportal/hazardmap/copyright/opendata.html#l2shinsuishin)

## 使用ライブラリ
* MapLibre GL JS https://github.com/maplibre/maplibre-gl-js
* protomaps/PMTiles https://github.com/protomaps/PMTiles/
* Turf.js https://turfjs.org/
* 地理院地図及び地理院地図Vectorのソース https://github.com/gsi-cyberjapan
