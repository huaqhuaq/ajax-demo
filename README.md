# ajax-demo

用原生 JS 写出一个 AJAX 请求

myButton.addEventListener('click', (e)=>{
  let request = new XMLHttpRequest()
  request.open('get', '/xxx') // 配置request
  request.send()
  request.onreadystatechange = ()=>{
    if(request.readyState === 4){
      if(request.status >= 200 && request.status < 300){

      }
    }
  }
})