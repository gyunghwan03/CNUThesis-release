컴파일 환경
===========

이 클래스는 TeXLive 2013 이후 버전에서 동작합니다.

이 버전 이후부터 koTeX이 기본 탑재돼 있습니다.

이전버전의 TeXLive에서 사용할 경우에는 koTeX을 따로 설치해주세요.


필수로 있어야 하는 파일
=======================

* 초록: abstract.tex
* 감사의 글: acknowledgement.tex

위 두 개의 파일은 내용만 수정하면 됩니다.

 * 논문 템플릿: CNUThesis.cls

템플릿 파일은 사용자가 만지지 않아도 되도록 최선을 다해서 만들었지만, 언제나 예외는 있기에 필요하면 수정하셔도 됩니다.

 * 논문 메인 파일:  thesis.tex

처음 한번만 고치면 챕터 추가 외에는 그다지 고칠 일이 없을겁니다.


본인에게 맞게 꼭 수정
=====================

* 논문 메인 파일 : thesis.tex

thesis.tex 파일 내부에 설명이 잘 되어 있으니, 따로 설명이 필요하지 않을 것 같습니다. 

* 참고문헌 목록 : library.bib

참고문헌 목록은 학술지 페이지의 BibTeX 형식으로 제공되는 데이타를 사용하면 됩니다.
예를들어 http://rmp.aps.org/abstract/RMP/v30/i2/p257_1 페이지에 들어가 보면 중간에 Export 라고 돼 있는 부분 오른쪽에 BibTeX 이라고 돼 있는 버튼을 눌러 다운받을 수 있게 돼 있는데, 그 정보들을 채워넣으면 됩니다. 논문 본문에서는 해당 파일의 첫번째 인자를 사용하면 됩니다. 제시한 예제에서는 첫 번째 인자가 RevModPhys.30.257 이므로, \cite{RevModPhys.30.257}와 같이 사용하면 됩니다.

컴파일 방법
===========

유닉스 환경에서는 `make`, 윈도우에서는 `make.bat`을 실행시키면 자동으로 컴파일이 되어 `thesis.pdf`파일이 생성됩니다. 중간에 뭔가 꼬여 처음부터 컴파일을 해야 할 일이 있다면, 유닉스 환경에서는 `make clean`, 윈도에어서는 `clean.bat`을 이용해서 초기화 할 수 있습니다. 이 때 사용자가 작성한 파일들은 날아가지 않으나 항상 조심하는게 좋으니 **백업을 강력하게 권장합니다.**

주의
====

이 템플릿 파일을 사용해서 발생하는 모든 문제에 대해서 템플릿 작성자들은 어떠한 책임도 지지 않습니다.

참고 자료
=========

http://library.korea.ac.kr/link/html/useThesesGuide03
