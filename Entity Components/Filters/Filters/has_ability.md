# has_ability  
エンティティ、オブジェクトが指定されたアビリティを持つ場合trueを返します。

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
<td>アビリティ名(必須)
<dl><dd><table class="wikitable">
<tbody><tr>
<th>オプション</th>
<th>説明
</th></tr>
<tr>
<td>worldbuilder<br>
EducationEditionのallowブロックとdenyブロックを、
設置できる状態(要検証)<sup><a href="#1">1</a></sup>
</td>
<td>
</td></tr>
<tr>
<td>invulnerable<br>
無敵(要検証)<sup><a href="#1">1</a></sup>
</td>
<td>
</td></tr>
<tr>
<td>flying<br>
飛行(要検証)<sup><a href="#1">1</a></sup>
</td>
<td>
</td></tr>
<tr>
<td>instabuild<br>
</td>
不明(要検証)<sup><a href="#1">1</a></sup>
<td>
</td></tr>
<tr>
<td>flySpeed<br>
飛行速度(要検証)<sup><a href="#1">1</a></sup>
</td>
<td>
</td></tr>
<tr>
<td>lightning<br>
帯電(要検証)<sup><a href="#1">1</a></sup>
</td>
<td>
</td></tr>
<tr>
<td>walkSpeed<br>
移動速度(要検証)<sup><a href="#1">1</a></sup>
</td>
<td>
</td></tr>
<tr>
<td>noclip<br>
スペクテイター(要検証)<sup><a href="#1">1</a></sup>
</td>
<td>
</td></tr>
<tr>
<td>mayfly<br>
クリエイティブ飛行(要検証)<sup><a href="#1">1</a></sup>
</td>
<td>
</td></tr>
<tr>
<td>mute<br>
チャットがミュート(要検証)<sup><a href="#1">1</a></sup>
</td>
<td>
</td></tr></tbody></table></dd></dl>
</td></tr></tbody></table></dd></dl>


# サンプルコード 
```json
{ "test": "has_ability", "subject": "self", "operator": "equals", "value": "instabuild" }
```
これは、エンティティ、オブジェクトがinstabuildを持つ際にtrueを返すフィルタです。  
デフォルト値を使うことで、省略して記述できます。  
```json
{ "test": "has_ability", "value": "instabuild" }
```  
[翻訳元](https://minecraft.gamepedia.com/Bedrock_Edition_entity_components_documentation#has_ability)  

<span id="1" style="font-size:x-small">1: 原文にこの記述はありません。</span>
