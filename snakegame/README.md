# 简易贪吃蛇游戏

一个基于 HTML、CSS 和 JavaScript 开发的网页版贪吃蛇游戏，支持经典的贪吃蛇玩法。

## 功能
- 玩家通过方向键（↑↓←→）控制蛇的移动方向
- 蛇吃到食物后会增长长度并生成新的食物
- 撞到自身时游戏结束
- 填满整个网格时获胜
- 边界采用穿越设计（从一边出去会从另一边进来）

## 如何运行
直接打开保存游戏代码的 HTML 文件（如 snakemaster.html）即可在浏览器中运行。

## 目前已知bug
在蛇身两格长及以上时，快速按动移动键会导致游戏失败，主要与定时器处理间隔内direction的多次处理有关，使蛇头判定到蛇头方向反向的身体，推测可以通过对direction的优化或蛇头碰撞的优化解决。


# Simple Snake Game
A web-based snake game developed with HTML, CSS, and JavaScript, featuring classic snake gameplay.

## Features
- Players can control the snake's direction using arrow keys (↑↓←→)
- The snake grows in length when it eats food, and new food is generated
- Game over when the snake hits itself
- Win by filling the entire grid with the snake
- Boundary wrapping (exiting one side enters from the opposite side)

## How to Run
Simply open the HTML file where the game code is saved (e.g., snakemaster.html) in a web browser.

## Known Bugs
When the snake's body is two or more cells long, rapidly pressing the movement keys can cause the game to end. This is mainly related to multiple direction changes within the timer interval, causing the snake's head to collide with the body in the opposite direction. It is speculated that this can be fixed by optimizing the direction handling or snake head collision detection.