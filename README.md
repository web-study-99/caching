# caching
서버와 클라이언트 캐싱

## 캐시 동작

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/a6ec37e7-c6b2-4d92-9cb4-d6a0cbec084b/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20221204%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20221204T140431Z&X-Amz-Expires=86400&X-Amz-Signature=7a2e400cee587661e22858308da561a9c5c4293e6a6fe9ea962c3b3fac1569e8&X-Amz-SignedHeaders=host&response-content-disposition=filename%3D%22Untitled.png%22&x-id=GetObject)

## 서버와 클라이언트간의 동기화

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/deb99474-0cc4-4d09-b2da-8979cc977a51/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20221204%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20221204T140443Z&X-Amz-Expires=86400&X-Amz-Signature=3c126ec6b8fdbb8c121deb76948bcd7e99ed16e35a245b6a39f45c164491b21b&X-Amz-SignedHeaders=host&response-content-disposition=filename%3D%22Untitled.png%22&x-id=GetObject)

<aside>
❓ 서버와 클라이언트 간에 서버의 데이터가 변경이 되었을때 cost 없이 real-time을 하는 방법?

</aside>

COST 없이 구현?

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/58919e80-ae8d-4d77-97c5-ad014617ee82/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20221204%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20221204T140454Z&X-Amz-Expires=86400&X-Amz-Signature=ab1f6728146120fea2e4ccf048f3eecbd0e1ec621c167ddec9a374be66f52ec0&X-Amz-SignedHeaders=host&response-content-disposition=filename%3D%22Untitled.png%22&x-id=GetObject)

구글 캘린더의 데이터를 Client에서 변경하였을 때 데이터의 변경 동기화? 

cost 없이 server에 캐싱을 사용하는 방법?

Google Notification API 사용 - 서버 데이터 변경될때 마다 알려줌

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/923cc095-1f22-43fe-9344-bae1b12e83d7/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20221204%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20221204T140507Z&X-Amz-Expires=86400&X-Amz-Signature=fa3af7f97caacae0269fca4302ee41d18b114175eb27a48e1fedae40c9143bc8&X-Amz-SignedHeaders=host&response-content-disposition=filename%3D%22Untitled.png%22&x-id=GetObject)

## Reference

[웹 서비스 캐시 똑똑하게 다루기](https://toss.tech/article/smart-web-service-cache) - toss tech

**[5 Ways to Sync Web and Server Data in Real Time](https://blog.bitsrc.io/5-ways-to-sync-web-and-server-data-in-real-time-3b5748ad2bf7)**
