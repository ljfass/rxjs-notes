# rxjs 笔记  
### 1.mergeMap 和 switchMap  
#### &emsp;https://cloud.tencent.com/developer/article/1533003  

### 2.在Angular项目中，常用到的订阅以及是否需要调用unsubscribe() 取消订阅，有以下几种：  
#### &emsp;Angular 中通过 HttpClient 执行 Http Request 返回的 Observables，订阅这些 Observables 拿到 API 返回的数据，不需要调用 unsubscribe() 取消订阅。
