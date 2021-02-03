# coding_skill_hitbox
## 当たり判定
当たり判定を、横方向と縦方向を別々に一旦考える  
### 横方向の判定処理
敵の原点が左側にある場合と、右側にある場合が想定出来るので、どちらも漏れがないように記述する
            me.x < enemy[count].x + enemy[count].width &&  
            enemy[count].x < me.x + me.width &&  
上記の式が２つともTrueじゃなければならない。
### 縦方向の判定処理
敵の原点が左側にある場合と、下側にある場合が想定出来るので、どちらも漏れがないように記述する  
            me.y < enemy[count].y + enemy[count].height&&  
            enemy[count].y < me.y + me.height    
  上記した4つの式が全てTrueだと「当たっている」判定になる

