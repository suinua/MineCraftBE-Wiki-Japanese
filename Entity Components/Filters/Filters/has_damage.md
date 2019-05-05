# has_damage  
テストの対象が、指定されたダメージを受けた時trueを返します。

# パラメーター

<dl><dd><table class="wikitable">
<tbody><tr>
<th>タイプ</th>
<th>名称</th>
<th>デフォルト値</th>
<th>説明
</th></tr>
<tr>
<td>String
</td>
<td>subject
</td>
<td>self
</td>
<td>このテストの条件対象。(オプション)
<dl><dd><table class="wikitable">
<tbody><tr>
<th>オプション</th>
<th>説明
</th></tr>
<tr>
<td>self
</td>
<td>テストを呼び出したエンティティ、オブジェクト
</td></tr>
<tr>
<td>other
</td>
<td>イベント対話中で、テストを呼び出していないエンティティ、オブジェクト
</td></tr>
<tr>
<td>parent
</td>
<td>テストを呼び出したエンティティ、オブジェクトの親状態にあるエンティティ、オブジェクト
</td></tr>
<tr>
<td>player
</td>
<td>イベント対話に関与したプレイヤー
</td></tr>
<tr>
<td>target
</td>
<td>現在ターゲットになっているエンティティ、オブジェクト
</td></tr></tbody></table></dd></dl>
</td></tr>
<tr>
<td>String
</td>
<td>operator
</td>
<td>equals
</td>
<td>値を比較するための演算子。(オプション)
<dl><dd><table class="wikitable">
<tbody><tr>
<th>Options</th>
<th>説明
</th></tr>
<tr>
<td>&gt;=
</td>
<td>value以上であればtrueを返します
</td></tr>
<tr>
<td>equals
</td>
<td>valueと等しければtrueを返します
</td></tr>
<tr>
<td>&lt;&gt;
</td>
<td>valueと等しくなければtrueを返します
</td></tr>
<tr>
<td>==
</td>
<td>valueと等しければtrueを返します
</td></tr>
<tr>
<td>=
</td>
<td>valueと等しければtrueを返します
</td></tr>
<tr>
<td>not
</td>
<td>valueと等しくなければtrueを返します
</td></tr>
<tr>
<td>&lt;
</td>
<td>valueより小さければtrueを返します
</td></tr>
<tr>
<td>!=
</td>
<td>valueと等しくなければtrueを返します
</td></tr>
<tr>
<td>&gt;
</td>
<td>valueより大きければtrueを返します
</td></tr>
<tr>
<td>&lt;=
</td>
<td>value以下であればtrueを返します
</td></tr></tbody></table></dd></dl>
</td></tr>
<tr>
<td>String
</td>
<td>value
</td>
<td>
</td>
<td>ダメージタイプ(必須)
<dl><dd><table class="wikitable">
<tbody><tr>
<th>オプション</th>
<th>説明
</th></tr>
<tr>
<td>contact<br>
不明(要検証)<sup><a href="#1">1</a></sup>
</td>
<td>
</td></tr>
<tr>
<td>none<br>
不明(要検証)<sup><a href="#1">1</a></sup>
</td>
<td>
</td></tr>
<tr>
<td>lava<br>
マグマによるダメージ(要検証)<sup><a href="#1">1</a></sup>
</td>
<td>
</td></tr>
<tr>
<td>attack<br>
攻撃によるダメージ<sup><a href="#1">1</a></sup>
</td>
<td>
</td></tr>
<tr>
<td>override<br>
不明(要検証)<sup><a href="#1">1</a></sup>
</td>
<td>
</td></tr>
<tr>
<td>projectile<br>
投射物(要検証)<sup><a href="#1">1</a></sup>
</td>
<td>
</td></tr>
<tr>
<td>suffocation<br>
窒息ダメージ(要検証)<sup><a href="#1">1</a></sup>
</td>
<td>
</td></tr>
<tr>
<td>fall<br>
落下ダメージ(要検証)<sup><a href="#1">1</a></sup>
</td>
<td>
</td></tr>
<tr>
<td>starve<br>
空腹ダメージ(要検証)<sup><a href="#1">1</a></sup>
</td>
<td>
</td></tr>
<tr>
<td>fire<br>
火炎ダメージ(要検証)<sup><a href="#1">1</a></sup>
</td>
<td>
</td></tr>
<tr>
<td>fatal<br>
死亡(要検証)<sup><a href="#1">1</a></sup>
</td>
<td>テストの対象を倒すダメージ全て
</td></tr>
<tr>
<td>fire_tick<br>
不明(要検証)<sup><a href="#1">1</a></sup>
</td>
<td>
</td></tr>
<tr>
<td>drowning<br>
酸素不足によるダメージ(要検証)<sup><a href="#1">1</a></sup>
</td>
<td>
</td></tr>
<tr>
<td>block_explosion<br>
ブロック爆破ダメージ(要検証)<sup><a href="#1">1</a></sup>
</td>
<td>
</td></tr>
<tr>
<td>entity_explosion<br>
エンティティ爆破ダメージ(要検証)<sup><a href="#1">1</a></sup>
</td>
<td>
</td></tr>
<tr>
<td>void<br>
不明(要検証)<sup><a href="#1">1</a></sup>
</td>
<td>
</td></tr>
<tr>
<td>suicide<br>
自殺(要検証)<sup><a href="#1">1</a></sup>
</td>
<td>
</td></tr>
<tr>
<td>magic<br>
魔法によるダメージ(要検証)<sup><a href="#1">1</a></sup>
</td>
<td>
</td></tr>
<tr>
<td>wither<br>
ウィザー(状態？)によるダメージ(要検証)<sup><a href="#1">1</a></sup>
</td>
<td>
</td></tr>
<tr>
<td>anvil<br>
不明(要検証)<sup><a href="#1">1</a></sup>
</td>
<td>
</td></tr>
<tr>
<td>thorns<br>
とげ(要検証)<sup><a href="#1">1</a></sup>
</td>
<td>
</td></tr>
<tr>
<td>falling_block<br>
落下ブロックによるダメージ(要検証)<sup><a href="#1">1</a></sup>
</td>
<td>
</td></tr>
<tr>
<td>piston<br>
ピストンによるダメージ(要検証)<sup><a href="#1">1</a></sup>
</td>
<td>
</td></tr>
<tr>
<td>fly_into_wall<br>
壁に衝突した際のダメージ(要検証)<sup><a href="#1">1</a></sup>
</td>
<td>
</td></tr></tbody></table></dd></dl>
</td></tr></tbody></table></dd></dl>


# サンプルコード 
```json
{ "test": "has_damage", "subject": "self", "operator": "equals", "value": "fatal" }
```
これは、self(テストを呼び出したエンティティ、オブジェクト)が死亡するダメージを受けた際にtrueを返すフィルタです。  
デフォルト値を使うことで、省略して記述できます。  
```json
{ "test": "has_damage", "value": "fatal" }
```  
[翻訳元](https://minecraft.gamepedia.com/Bedrock_Edition_entity_components_documentation#has_damage)  

<span id="1" style="font-size:x-small">1: 原文にこの記述はありません。</span>