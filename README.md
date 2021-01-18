# 스크롤 트리거 모듈

- 셋팅
  1. main.js에 모듈 import
  2. Vue.prototype.$scroll에 import한 모듈넣기

- 메서드
  1. setSubject(sbuject, trigger)
      - subject : scroll 이벤트를 실행 시킬 주체
      - trigger : 주체의 트리거를 동작시킬 상위 높이(단위: 백분율)
  2. addEvent(subject, section, callback)
      - subject : 이벤트 발생이될 부모 주체
      - section : 트리거와 충돌 할 subject의 하위 section
      - callback : 해당 section 충돌 시 발생할 callback 메서드
  3. eventOn(subject)
      - subject : scroll 이벤트를 시작 할 주체
  4. clearEvent(subject)
      - subject : scroll 이벤트를 제거 할 주체(beforeDestory시 권장)