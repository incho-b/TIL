## **들어가기전에**

-   HTML5를 기준으로 한다.

-   Semantic Tag 란, 태그만 보고도 그 의미가 통하도록 하는 태그이다.

-   태그는 `<tag> </tag>` 의 양식으로 작성하며, 빈 태그 혹은 닫는 태그가 없는 태그의 경우에는 `<tag />` 의 양식으로 작성한다.

    <br /> <br />

# Semantic Tag

## `<header>`

-   페이지의 제목 혹은 가장 상단의 헤더 부분을 나타낼 때 사용한다.

## `<nav>`

-   현재 페이지 내, 또는 다른 페이지로의 링크를 보여주는 메뉴, 목차, 색인 등에 사용한다.

## `<h1> ~ <h6>`

-   `<h1>`은 가장 중요한 제목이므로 전체 페이지의 목적을 설명한다.
-   여러 개를 써도 오류는 나지 않겠지만, 단일 `<h1>`이 모범 사례로 꼽히며, 페이지 당 하나의 `<h1>`만 사용하는 것을 권장한다.

## `<main>`

-   페이지의 가장 주된 내용을 가지며, 기본적으로 1페이지당 1개의 main 요소를 갖는다.

## `<section>`

-   HTML 문서의 독립적인 구획을 나타내며, 더 적합한 의미를 가진 요소가 없을 때 사용한다.
-   각각의 `<section>`을 식별할 수단이 필요며, 주로 제목(`<h1> - <h6>`) 요소를 `<section>`의 자식으로 포함하는 방법을 사용한다.
-   ```html
    이전
    <div>
        <h2>Heading</h2>
        <img>some image</img>
    </div>

    이후
    <section>
        <h2>Heading</h2>
        <img>some image</img>
    </section>
    ```

## `<article>`

-   문서, 페이지, 애플리케이션, 또는 사이트 안에서 독립적으로 구분해 배포하거나 재사용할 수 있는 구획으로, 블로그 글, 뉴스기사 등에 사용.
-   각각의 `<article>`을 식별할 수단이 필요며, 주로 제목(`<h1> - <h6>`) 요소를 `<article>`의 자식으로 포함하는 방법을 사용한다.

## `<aside>`

-   문서의 주요 내용과 간접적으로만 연관된 부분을 나타낸다.
-   주로 사이드바 혹은 콜아웃 박스로 표현한다.

## `<footer>`

-   페이지의 가장 아랫부분에 사이트맵, 사이트 혹은 사업자 정보, 저작권 정보를 포함한다.

## `<address>`

-   가까운 HTML 요소의 사람, 단체, 조직 등에 대한 연락처 정보를 나타낸다.
-   `<address>` 요소의 콘텐츠가 제공하는 연락처 정보는 현재 맥락에 적절한 아무 형태나 취할 수 있다.
-   반드시 포함해야 하는 정보는 연락처가 가리키는 개인, 조직, 단체의 이름이다.
-   ```html
    <address>
    	<a href="mailto:jim@rock.com">jim@rock.com</a><br />
    	<a href="tel:+13115552368">(311) 555-2368</a>
    </address>
    ```

## `<detail>`

-   "열림" 상태일 때만 내부 정보를 보여주는 정보 공개 위젯을 생성한다.
-   요약이나 레이블은 `<summary>` 요소를 통해 제공할 수 있다.
-   ```html
    <details open>
    	<!-- defualt => open: false -->
    	<summary>Overview</summary>
    	<ol>
    		<li>Cash on hand: $500.00</li>
    		<li>Current invoice: $75.30</li>
    		<li>Due date: 5/6/19</li>
    	</ol>
    </details>
    ```

## `<summary>`

-   `<detail>` 요소의 공개 상자에 대한 요약, 캡션 또는 범례를 지정한다.
-   `<summary>` 요소를 클릭하면 부모 `<detail>` 요소의 상태가 열리거나 닫힌다.

    <br />

## - Gourp Tag

## `<hgroup>`

-   문서 구획의 다단계 제목을 나타며, 다수의 `<h1> - <h6>` 요소를 묶을 때 사용한다.
-   ```html
    <hgroup>
    	<h1>Calculus I</h1>
    	<h2>Fundamentals</h2>
    </hgroup>
    <p>
    	This course will start with a brief introduction about the limit of a function. Then we will describe how the idea of derivative
    	emerges in the Physics and Geometry fields. After that, we will explain that the key to master calculus is …
    </p>
    ```

## `<colgroup>`

-   표의 열을 묶는 그룹을 정의한다
-   ```html
    <table>
    	<caption>
    		Superheros and sidekicks
    	</caption>
    	<colgroup>
    		<col />
    		<col span="2" class="batman" />
    		<col span="2" class="flash" />
    	</colgroup>
    	<tr>
    		<td> </td>
    		<th scope="col">Batman</th>
    		<th scope="col">Robin</th>
    		<th scope="col">The Flash</th>
    		<th scope="col">Kid Flash</th>
    	</tr>
    	<tr>
    		<th scope="row">Skill</th>
    		<td>Smarts</td>
    		<td>Dex, acrobat</td>
    		<td>Super speed</td>
    		<td>Super speed</td>
    	</tr>
    </table>
    ```

## `<optgroup>`

-   `<select>` 요소의 옵션을 묶을 수 있다.
-   ```html
    <label for="dino-select">Choose a dinosaur:</label>
    <select id="dino-select">
    	<optgroup label="Theropods">
    		<option>Tyrannosaurus</option>
    		<option>Velociraptor</option>
    		<option>Deinonychus</option>
    	</optgroup>
    	<optgroup label="Sauropods">
    		<option>Diplodocus</option>
    		<option>Saltasaurus</option>
    		<option>Apatosaurus</option>
    	</optgroup>
    </select>
    ```
