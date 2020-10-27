# My First README

**** CSS and HTML will be revised later ****

Repo explaining Tic Tac Toe for andrewemcmanus

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
## javascript:
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


# CSS (to be revised):
```css
body{
  margin:0px;
  padding:0px;
}

h1 {
  color: purple;
  text-align: center;
}

.row {
  position: relative;                                           
}
.square {
                   /* flex: 0 0 32%;  don't grow, don't shrink, width */
  height: 50px;
  width: 50px;
  display: block;
  margin-bottom: 5px;
  background-color: #999;
  text-align: center;
}
```
# HTML (to be revised):
```html
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>tic tac toe</title>
  <link rel="stylesheet" type="text/css" href="css/style.css">
</head>
<body>
  <h1>tic tac toe</h1>
  <div class="grid">
    <div class="row">
      <div class="square" id="1"></div>
      <div class="square" id="2"></div>
      <div class="square" id="3"></div>
    </div>
    <div class="row">
      <div class="square" id="4"></div>
      <div class="square" id="5"></div>
      <div class="square" id="6"></div>
    </div>
    <div class="row">
      <div class="square" id="7"></div>
      <div class="square" id="8"></div>
      <div class="square" id="9"></div>
    </div>
    

  </div>
  <script type="text/javascript" src="js/app.js"></script>
</body>
</html>
```
# table:
| functions | Description |
| ----------- | ----------- |
| Header | Title |
| Paragraph | Text |

## Functions:
| functions | Description |
| ----------- | ----------- |
| arrayEquals | compares two arrays |
| checkWinner | checks player choices against winning combinations |
| fillSquareOne | adds X or O to square |
| fillSquareTwo |                       |
| fillSquareThree |                     |
| fillSquareFour |                      |
| fillSquareFive |                      |
| fillSquareSix |                       |
| fillSquareSeven |                     |
| fillSquareEight |                     |
| fillSquareNine |                      |

