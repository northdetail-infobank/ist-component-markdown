# BaseButton

## What

汎用ボタンの出力を行う<br>
（\<button> の機能を請け負う）

ボタン上に表示するテキストやクリック時のイベント、デザイン等を設定可能。

## How

### ◆ 使用例

```html
<base-button
  :props-text="Default"
  :props-disabled="false"
  :props-block="false"
  :props-color="#fff"
  :props-before-icon="home"
  :props-after-icon="home"
  :props-dark="false"
  :props-outline="false"
  :props-herf="http://example.com/"
  :props-type="button"
  :props-class=""
  :props-radius="5px"
  @onClick="onClick"
/>
```

### ◆ プロパティ(props)

| 名称              | 型      | 初期値      | 必須 | 概要                                      |
| ----------------- | :------ | :---------- | ---- | ----------------------------------------- |
| props-text        | string  | '' (空文字) | ◯    | ボタン上に表示する文字列を設定する        |
| props-color       | string  | '' (空文字) |      | ボタン色を設定する                        |
| props-disabled    | boolean | false       |      | 非活性に設定する                          |
| props-block       | boolean | false       |      | ブロック要素に設定する                    |
| props-before-icon | string  | '' (空文字) |      | propsTextの前に表示するアイコンを設定する |
| props-after-icon  | string  | '' (空文字) |      | propsTextの後に表示するアイコンを設定する |
| props-dark        | boolean | false       |      | テーマカラーをDarkに設定する              |
| props-outline     | boolean | false       |      | ボタンを境界線で表現する                  |
| props-herf        | string  | '' (空文字) |      | クリック後の遷移先を設定する              |
| props-type        | string  | 'button'    |      | ボタンの属性を設定する                    |
| props-class       | string  | '' (空文字) |      | ボタンに指定するclassを設定する           |
| props-radius      | string  | '5px'       |      | 角丸を指定する                            |

### ◆ 算出プロパティ(computed)

| 名称   | 概要                                       |
| ------ | ------------------------------------------ |
| styles | 「props-radius」を非同期で受け取り返却する |

### ◆ 関数(methods)

| 名称    | 引数 | 返り値 | 概要                       |
| ------- | ---- | ------ | -------------------------- |
| onClick | なし | なし   | クリックイベントを実行する |


## GitHub

* Component | BaseButton.vue<br>
https://github.com/scalar-labs/information-banking/blob/feature/ticket57408/ist-components/components/atoms/BaseButton.vue

* Markdown | BaseButton.md<br>
https://github.com/scalar-labs/information-banking/blob/feature/ticket57408/ist-components/stories/atoms/notes/BaseButton.md