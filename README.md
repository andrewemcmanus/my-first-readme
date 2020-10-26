# My First README

Repo explaining Tic Tac Toe for andrewemcmanus

```javascript
const handleWin = (letter) => {
  gameIsLive = false;
  if (letter === "x") {
    statusDiv.innerHTML = `${letterToSymbol(letter)} has won!`;
  } else {
    statusDiv.innerHTML = `<span>${letterToSymbol(letter)} has won!</span>`;
  }
};
```
## Steps to install on local computer
1. Go [repo](https://github.com/andrewemcmanus) 
2. `Fork` and `clone` the repo
3.  Clone to local machine
```text
git clone https://github.com/andrewemcmanus
```
4. cd to `tic-tac-toe` directory
5. Open `index.html` in browser
```text
open index.html
```
# CSS Code:
```css
.grid {
    background-color: salmon;
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows: repeat(3, 1fr);
    gap: 15px;
    margin-top: 50px;
}
```
#HTML:
```html
<div class="grid">
    <div class="box" id="box-1"></div>
    <div class="box" id="box-2"></div>
    <div class="box" id="box-3"></div>
    <div class="box" id="box-4"></div>
    <div class="box" id="box-5"></div>
    <div class="box" id="box-6"></div>
    <div class="box" id="box-7"></div>
    <div class="box" id="box-8"></div>
    <div class="box" id="box-9"></div>
</div>
```
#table:
| functions | Description |
| ----------- | ----------- |
| Header | Title |
| Paragraph | Text |

## Functions:
| functions | Description |
| ----------- | ----------- |
| arrayEquals | Title |
| checkWinner | Text |
| fillSquareOne | Text |
| fillSquareTwo | Text |
| fillSquareThree | Text |
| fillSquareFour | Text |
| fillSquareFive | Text |
| fillSquareSix | Text |
| fillSquareSeven | Text |
| fillSquareEight | Text |
| fillSquareNine | Text |

```javascript
// callback functions:
function arrayEquals(a, b) {
    // a replacement for === for arrays
    return Array.isArray(a) &&
      Array.isArray(b) &&
      a.length === b.length &&
      a.every((val, index) => val === b[index]);
  }
function checkWinner () {
    // compares player choice arrays to possible winning combos:
    let winner = null;
    for (let i = 0; i < combos.length; i++) {
        if (arrayEquals(player1Selections, combos[i])) {
            console.log("Player 1 wins!");
            winner = 1;
        } else if (arrayEquals(player2Selections, combos[i])) {
            console.log("Player 2 wins!");
            winner = 2;
        }
    }
    return winner;
    }
// functions to mark each square an with X or O, alternating turns:
function fillSquareOne() {
    if (turn % 2 !== 0) {
        document.getElementById("1").innerText = "X";
        player1Selections.push(0);
        } else if (turn % 2 === 0) {
        document.getElementById("1").innerText = "O";
        player2Selections.push(0);
    }
    checkWinner();
    turn += 1;
    return turn; 
    }
function fillSquareTwo() {
        if (turn % 2 !== 0) {
            document.getElementById("2").innerText = "X";
            player1Selections.push(1);
            } else if (turn % 2 === 0) {
            document.getElementById("2").innerText = "O";
            player2Selections.push(1);
        }
        checkWinner();
        turn += 1;
        return turn; 
        }
function fillSquareThree() {
    if (turn % 2 !== 0) {
        document.getElementById("3").innerText = "X";
        player1Selections.push(2);
    } else if (turn % 2 === 0) {
        document.getElementById("3").innerText = "O";
        player2Selections.push(2);
    }
    checkWinner();
    turn += 1;
    return turn;
}        
function fillSquareFour () {
    if (turn % 2 !== 0) {
        document.getElementById("4").innerText = "X";
        player1Selections.push(3);
    } else if (turn % 2 === 0) {
        document.getElementById("4").innerText = "O";
        player2Selections.push(3);
    }
    checkWinner();
    turn += 1;
    return turn;
}
function fillSquareFive () {
    if (turn % 2 !== 0) {
        document.getElementById("5").innerText = "X";
        player1Selections.push(4);
    } else if (turn % 2 === 0) {
        document.getElementById("5").innerText = "O";
        player2Selections.push(4);
    }
    checkWinner();
    turn += 1;
    return turn;
}
function fillSquareSix () {
    if (turn % 2 !== 0) {
        document.getElementById("6").innerText = "X";
        player1Selections.push(5);
    } else if (turn % 2 === 0) {
        document.getElementById("6").innerText = "O";
        player2Selections.push(5);
    }
    checkWinner();
    turn += 1;
    return turn;
}
function fillSquareSeven () {
    if (turn % 2 !== 0) {
        document.getElementById("7").innerText = "X";
        player1Selections.push(6);
    } else if (turn % 2 === 0) {
        document.getElementById("7").innerText = "O";
        player2Selections.push(6);
    }
    checkWinner();
    turn += 1;
    return turn;
}
function fillSquareEight () {
    if (turn % 2 !== 0) {
        document.getElementById("8").innerText = "X";
        player1Selections.push(7);
    } else if (turn % 2 === 0) {
        document.getElementById("8").innerText = "O";
        player2Selections.push(7);
    }
    checkWinner();
    turn += 1;
    return turn;
}
function fillSquareNine () {
    if (turn % 2 !== 0) {
        document.getElementById("9").innerText = "X";
        player1Selections.push(8);
    } else if (turn % 2 === 0) {
        document.getElementById("9").innerText = "O";
        player2Selections.push(8);
    }
    checkWinner();
    turn += 1;
    return turn;
}
```
