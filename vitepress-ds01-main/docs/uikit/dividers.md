---
layout: doc
sidebar: true
---
# Dividers 分隔線
> 通常以水平或垂直線條呈現，並可搭配文字或圖示，提升視覺層次感與可讀性。

<script setup>
    import Dividers from '../components/Dividers.vue'
</script>
## 元件預覽
<Dividers />

## 程式碼
::: code-group
```html [html]
  <div class="l-divider">
    <hr class="l-divider-horizontal">
    <hr class="l-divider-straight">
  </div>
```
```css [css]
.l-divider{
    position: relative;
    display: inline-block;
    width: 100%;
}
.l-divider-horizontal { 
    border-top: 1px solid;
    width: 100%;
}
.l-divider-straight{
    display: inline-block;
    margin: 0 0px;
    border-top: none;
    border-left: 1px solid;
    height: 100%;
}
```
## 元件規範
<div class="table-responsive">
    <table class="table table-bordered w1000">
        <thead class="bg-primary-8">
            <tr>
                <th scope="col" style="width: 15%;"></th>
                <th scope="col" colspan="3">All media</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td rowspan="2" class="bg-primary-2" scope="row">
                    <p class="text-gray-11">Type1</p>
                </td>
                <td style="padding: 40px 20px;">
                    <img src="./overview/img/dividers-1.png" alt="" width=400px;>
                </td>
            </tr>
            <tr>
                <td>
                    <b>寬度自行調整</b>
                    <ul class="pl-3 my-1">
                        <li>border:solid 1px #d9d9d9</li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td rowspan="2" class="bg-primary-2" scope="row">
                    <p class="text-gray-11">Type2</p>
                </td>
                <td style="padding: 40px 20px;">
                    <img src="./overview/img/dividers-2.png" alt="" width=400px;>
                </td>
            </tr>
            <tr>
                <td>
                    <b>寬度自行調整</b>
                    <ul class="pl-3 my-1">
                        <li>border:solid 1px #bde3e2</li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td rowspan="2" class="bg-primary-2" scope="row">
                    <p class="text-gray-11">標題+分隔線</p>
                </td>
                <td style="padding: 30px 20px;">
                    <img src="./overview/img/dividers-3.png" alt="" width=360px;>
                </td>
            </tr>
            <tr>
                <td>
                    <b>寬度自行調整<br>標題分隔線間距4px</b><br>
                    <b>標題</b>
                    <ul class="pl-3 my-1">
                        <li>font-size:20px</li>
                        <li>color:#009a18</li>
                    </ul>
                    <b>分隔線</b>
                    <ul class="pl-3 my-1">
                        <li>border:solid 1px #bde3e2</li>
                    </ul>
                </td>
            </tr>
        </tbody>
    </table>
</div>