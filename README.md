# War-Record
War Record
title="高级飞行员";
else if(x == 2)
title="王牌飞行员";
cout<<title;
rankf = rank;
void Game::Playing()
//HANDLE MFUN;
//MFUN= CreateThread(NULL, 0, MusicFun, NULL, 0, NULL); 
drawEnemy();
drawPlane();
int flag_bullet = 0;
int flag_enemy = 0;
while(1)
Sleep(8);
if(_kbhit())
char x = _getch();
if ('a' == x || 's' == x || 'd' == x || 'w' == x)
drawPlaneToNull();
planeMove(x);
drawPlane();
judgePlane();
else if ('p' == x)
Pause();
lse if( 'k' == x)
Shoot();
else if( 'e' == x)
//CloseHandle(MFUN);
GameOver();
break
/* 处理子弹 */
if( 0 == flag_bullet )
bulletMove();
drawBulletToNull();
drawBullet();
judgeEnemy();
flag_bullet++;
if( 5 == flag_bullet )
flag_bullet = 0;
/* 处理敌人 */
if( 0 == flag_enemy )
drawEnemyToNull();
enemyMove();
rawEnemy();
judgePlane();
flag_enemy++;
if( flag_enemy >= rank )
