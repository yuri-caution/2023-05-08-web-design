# 웹디자인 기능사 시험 연습


#### inline 요소는 block 요소를 감쌀 수 없음
#### 그러나 a 태그는 inline 요소임에도 무엇이든 감쌀 수 있음.


### 말줄임표 넣기
```
.tab_cont .notice li a {
    display: block;
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;

}
```

### 가로 세로 비율 유지하며 100% 크기
```
.banner img {
    display: block;
    width: 100%;
    height: 100%;
    object-fit: cover;
}
```

## 팝업창 띄우기
```
<div class="modal">
        <h2>지나가는 둘</h2>
        <p>노새, 지나가는 둘 한 당신은 듯합니다. 쓸쓸함과 별 노루, 풀이 속의 이제 이웃 시인의 그리워 까닭입니다. 가을로 이름과 가난한 별 까닭이요, 된 버리었습니다. 까닭이요, 언덕 이웃 이름과, 다하지 무성할 멀리 듯합니다. 헤일 시인의 계절이 가난한 하나 하나의 옥 시와 봅니다. 위에 경, 무성할 멀리 우는 오면 내린 봅니다. 밤을 별 하나에 비둘기, 있습니다. 이름과, 했던 쓸쓸함과 그리워 없이 묻힌 불러 까닭입니다. 내일 차 청춘이 오는 까닭이요, 아직 있습니다.</p>
        <a href="#" class="close">닫기</a>
    </div>
```
```
/* modal  */
.modal {
    position: fixed;
    top: 0;
    left: 0;
    width: 600px;
    height: 460px;
    background-color: #fff;
    border: 1px solid #666;
    padding: 50px 40px;
}

.modal h2 {
    font-size: 36px;
    margin-bottom: 30px;
}

.modal p {
    line-height: 1.8;
    font-size: 16px;
}

.modal .close {
    display: block;
    width: 100px;
    height: 40px;
    background-color: #ddd;
    text-align: center;
    line-height: 40px;
    position: absolute;
    bottom: 50px;
    right: 40px;
}
```