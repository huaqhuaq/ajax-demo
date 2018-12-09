# ajax-demo

用原生 JS 写出一个 AJAX 请求

```
let request = new XMLHttpRequest()
request.open('get', '/xxx') // 配置request
request.send()
request.onreadystatechange = ()=>{
if(request.readyState === 4){ 
  if(request.status >= 200 && request.status < 300){
    console.log('说明请求成功')
  }else if(request.status >= 400){
    console.log('说明请求失败') 
  }
}
}
```