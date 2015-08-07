### 字符串相关

#### 生成随机字符串

```php
<?php
    function randstr($len) {
        $c = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789";
        $ret = "";
        $charlen = strlen($c);
        for($i=0; $i<$len; $i++) { 
            $ret.= $c[rand()%$charlen]; 
        }
        return $ret; 
	}
?>
```

### switch case 弱类型比较
```php
$a = 1;
switch (true) {
    case true === $a:
        echo 'success';
        break;
    default :
        echo 'fail';
}
```
