PiniEngine
=============
피니엔진은 비주얼 노벨 게임 제작도구입니다. 

[![IMAGE ALT TEXT](http://img.youtube.com/vi/5FD2cSPqFLE/0.jpg)](http://www.youtube.com/watch?v=5FD2cSPqFLE "피니엔진 프리뷰 트레일러")

LNX 스크립트를 이용하여 게임을 개발하며 개발 및 빌드를 도와주는 에디터가 동봉되어있습니다.
피니에디터를 이용하여 개발 스크립트를 작성하고 작성된 스크립트는 PLY를 통해 컴파일 되며 만들어진 실행파일은 cocos2d-x엔진을 통해 실행됩니다.

LNX
-------------
LNX는 피니엔진용 스크립트언어입니다. 한글로 스크립팅할 수 있다는 특징이있습니다.
LNX의 형태는 아래와 같습니다.
<pre><code>
#파라미터 알려줌
:야근시작
[대화 이름="김똘똘"]
;으윽! 야근인건가요?

직원수 = $프로그래머 + $그래픽 + $사운드 + $기획자 + $QA + $운영자
@조건 직원수 == 0:
	[대화 이름="김똘똘"]
	;하지만 야근을 할 직원이 없군요...
	>>주메뉴시작

[독백]
;야근을 하게되면 시간을 추가로 얻을 수 있습니다 하지만 사원들은 애사심이 떨어지고 애사심이 너무 떨어지면..
;퇴사를 하기도 합니다. 보너스로 달랠 수 있기는 합니다만.
;
;<연결 "야근10">10시간 야근</연결>
;<연결 "야근20">20시간 야근</연결>
;<연결 "야근40">40시간 야근</연결>
;
;<연결 "야근포기">그만두자</연결>
;
</code></pre>