# Markdown

마크다운(markdown)은 일반 텍스트 기반의 경량 마크업 언어다. 일반 텍스트로 서식이 있는 문서를 작성하는 데 사용되며, 일반 마크업 언어에 비해 문법이 쉽고 간단한 것이 특징이다. HTML과 리치 텍스트(RTF) 등 서식 문서로 쉽게 변환되기 때문에 응용 소프트웨어와 함께 배포되는 README 파일이나 온라인 게시물 등에 많이 사용된다. <br />
보통 Github의 README 파일로 사용.

# h1 tag

## h2 tag

### h3 tag

#### h4 tag

##### h5 tag

###### h6 tag

    # h1 tag
    ## h2 tag
    ### h3 tag
    #### h4 tag
    ##### h5 tag
    ###### h6 tag

    This is a h1
    =============

    This is a h2
    -------------

    # 의 개수, = - 로 제목을 표기할 수 있다.

## Blockquote

    This is a first blockqute.
    > tab으로 들여쓰기를 하면 블록안에 글이 작성된다.

> This is a first blockqute.
>
> > This is a second blockqute.
> >
> > > This is a third blockqute.

    > This is a first blockqute.
    >   > This is a second blockqute.
    >   >   > This is a third blockqute.

## List

### ol

1. 첫번째
2. 두번째
3. 세번째

```
    1. 첫번째
    2. 두번째
    3. 세번째
```

### ul

-   첫번째
    -   두번째
        -   세번째

```
* 첫번째
    - 두번째
        + 세번째

    * - + 중 어느것을 사용해도 상관이 없고,
    들여쓴 위치에 따라 리스트 스타일이 적용된다.
```

## Code

```html
<h1>hello</h1>
<div>This is a <span>Code</span>.</div>
```

```css
span {
    color: red;
}
```

```javascript
document.querySelector('div');
```

    ```html
    <h1>hello</h1>
    <div>This is a <span>Code</span>.</div>
    ```

    ```css
    span {
        color: red;
    }
    ```

    ```javascript
    document.querySelector('div');
    ```

    ```language
    언어 이름을 입력해주면 조금더 코드를 보기 편하게 출력해 준다.
    ```

## hr tag

---

    ---

## Link

[Google](https://google.com/, 'Google')

    [Google](https://google.com/, 'Google')

## Text Decoration

_single underscores_

**double asterisks**

~~cancelline~~

    _single underscores_
    **double asterisks**
    ~~cancelline~~

    *single asterisks*
    __double underscores__
    도 사용이 가능하지만, prettier 사용시
    _single underscores_
    **double asterisks**
    과 중복으로 자동변환된다.

## Img

<img src="https://incho-b.github.io/portfolio/img/IMG_0300.PNG" width="200px" height="" title="px(픽셀) 크기 설정" alt="Penguni" />

    <img src="https://incho-b.github.io/portfolio/img/IMG_0300.PNG" width="200px" height="" title="px(픽셀) 크기 설정" alt="Penguni" />
    width 값과 height 값을 모두 입력하면 이미지 비율에 따라 찌그러져 보일 수 있다.
