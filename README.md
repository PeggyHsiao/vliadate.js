# validate.js
用來驗證表單的JS函式庫。

## 安裝
### CDN
也需要嵌入`JQuery`檔案才可以正常使用`validate.js`。
```
<script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"</script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery-validate/1.19.1/jquery.validate.min.js"></script>
```
首先在HTML中寫入要呈現的表單欄位，這裡的CSS套用`Bootstrap4`。
```
// index.html

<form id="form-content">
    <h2>validate.js範例表單</h2>
    <hr>
    <div class="row">
        <div class="col-md-12">
            <label for="email" class="form-group">電子信箱</label>
            <input type="text" class="form-control" id="email" name="email" placeholder="請輸入電子信箱">
        </div>
    </div>

    <div class="row">
        <div class="col-md-6">
            <label for="password" class="form-group">密碼</label>
            <input type="password" class="form-control" id="password" name="password">
        </div>
        <div class="col-md-6">
            <label for="password-again" class="form-group">確認密碼</label>
            <input type="password" class="form-control" id="password-again" name="password-again">
        </div>
    </div>
    <button type="submit" class="btn btn-primary">Sumbit</button>
</form>
```
`<label for="OOO">`要和`<input id="OOO">`對應，而`<input name="XXX">`則是要和.js檔的名稱相同，反正大家都取一樣的也無所謂。