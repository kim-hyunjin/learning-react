# 15장 Context API
Context API는 리액트 프로젝트에서 전역적으로 사용할 데이터가 있을 때 유용한 기능이다.
- 사용자 로그인 정보
- 애플리케이션 환경 설정
- 테마 등

리덕스, 리액트 라우터, styled-components 등의 라이브러리는 Context API를 기반으로 구현되어있다.
```
<ColorContext.Consumer>
  {value => (
    <div style={{
      width: '64px',
      height: '64px',
      background: value.color
    }}>
    </div>
  )}
</ColorContext.Consumer>
```
Consumer 사이에 중괄호를 열어 그 안에 함수를 넣어줌. - Function as a child, Render Props.