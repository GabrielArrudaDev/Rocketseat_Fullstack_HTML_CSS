# Existem 9 propriedades fundamentais:

## 6 aplicadas em container

- `align-content`
- `justify-content`
- `place-content` // aplica os dois de uma vez

 ---

- `align-items`
- `justify-items`
- `place-items` // aplica os dois de uma vez


## 3 aplicadas em items

- `align-self`
- `justify-self`
- `place-self` // aplica os dois de uma vez

# Podemos separar em 3 grupos :

- `align`
- `justify`
- `place`

E cada um deles irá observar o :
- conteúdo do elemento `content`
- itens do elemento `items`
- próprio elemento `self`

# Animation

## HTML:

`<div class="square"></div>`

## CSS:

`body{`

    - background-color: mediumpurple;

`}`

`.square {`

    - width: 4rem;

    - height: 4rem;

    - background-color: white;

    - opacity: .6;
`}`

`.square {`

    - animation-name: move, blink;

    - animation-duration: 1s, 200ms;

    - animation-fill-mode: forwards;

    - animation-direction: alternate;

    - animation-iteration-count: infinite;

    - /* animation-delay: 2s; */

    - animation-timing-function: steps(10);

`}`

---
*Shorthand:*

*animation: move 1s forwards alternate infinite, blink 100ms infinite;*

---

`}`

`.square:hover {`
    - animation-play-state: paused;

`}`

`@keyframes move {`

    - /* to */
    - 100% {
      - transform: translateX(calc(100vw - 100% - 16px));
      }

`}`

`@keyframes blink {`

    - 0%, 100% {
      - opacity: 0.6;
      }

    - 50% {
      - opacity: 1;
      }

`}`
