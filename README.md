# rxjs 笔记  
### 1.mergeMap 和 switchMap  
#### &emsp;https://cloud.tencent.com/developer/article/1533003  

### 2.在 Angular 项目中，常用到的订阅以及是否需要调用 unsubscribe() 取消订阅，有以下几种：  
#### &emsp;Angular 中通过 HttpClient 执行 Http Request 返回的 Observables，订阅这些 Observables 拿到 API 返回的数据，不需要调用 unsubscribe() 取消订阅。  
#### &emsp;Angular AsyncPipe，不需要调用 unsubscribe()取消订阅。  
#### &emsp;通过 Subject，BehaviorSubject，AsyncSubject，ReplaySubject 在各个 Component 之间通信，需要调用 unsubscribe()取消订阅。  
#### &emsp;RxJS 自带的一些操作符：take，takeWhile，first 等等，不需要调用 unsubscribe()取消订阅。   
#### &emsp;通过 HttpClient 执行 Http Request 返回的 Observable 是 Cold Observable。  

### 3.Cold vs Hot  
#### 数据生产者 vs 数据消费者  
#### &emsp;数据生产者是指 Observable(可观察对象)，产生数据的一方。   
#### &emsp;数据消费者是指 Observers(观察者)，接收数据的一方。
