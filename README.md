# Hyperledger-study-13

하이퍼레져 앱 만들기 실습 13일차 - 태그 Components화 시키기

1. 12일차 예제 앱을 활용

2. Html을 구성하는 태그(header, nav, article)를 Components화 시키기

3. header 생성

        <header>
          <h1>WEB</h1>
          World wide web!
        </header>
        
4. nav 생성

        <nav>
          <ul>
              <li><a href="1.html">HTML</a></li>
              <li><a href="2.html">CSS</a></li>
              <li><a href="3.html">JavaScript</a></li>
          </ul>
        </nav>

5. article 생성

        <article>
          <h2>HTML</h2>
          HTML is HyperText Markup Language.
        </article>

6. App.js 실행

7. <header> Component 만들기

        class Subject extends Component {
          render() {
            return(
              <header>
                <h1>WEB</h1>
                World wide web!
              </header>
            );
          }
        }
        
8. <nav> Component 만들기
  
        class Nav extends Component {
          render(){
            return(
              <nav>
                <ul>
                    <li><a href="1.html">HTML</a></li>
                    <li><a href="2.html">CSS</a></li>
                    <li><a href="3.html">JavaScript</a></li>
                </ul>
              </nav>
            );
          }
        }  

9. <article> Component 만들기

        class ART extends Component {
          render(){
            return(
              <article>
                <h2>HTML</h2>
                HTML is HyperText Markup Language.
              </article>
            );
          }
        }

10. Components 출력

        class App extends Component {
          render() {
            return (
              <div className="App">
               <Subject></Subject>
               <Nav></Nav>
               <ART></ART>
              </div>
            );
          }  
        }

태그를 컴포넌트로 사용하는 이유는 가독성을 높이고, 일처리를 빠르게 하기 위해서이다.
