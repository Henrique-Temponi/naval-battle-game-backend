<p align="center">
<img alt="Naval Battle Game Logo" src="https://i.imgur.com/zvdHbWT.png" height="300px"/>
<h2 align="center"><strong align="center">Back end</strong></h2>
</p>

## [Check our Front end](https://github.com/alicecabral/naval-battle-game-frontend)

## Members

- [alicecabral](https://github.com/alicecabral)
- [axell-brendow](https://github.com/axell-brendow)
- [HRKings](https://github.com/HRKings)
- [Henrique-Temponi](https://github.com/Henrique-Temponi)

## Technologies

<a href="https://www.docker.com/"><img alt="Docker" src="https://avatars0.githubusercontent.com/u/5429470?s=200&v=4" height="60px"></a>

<a href="https://www.postgresql.org/"><img alt="PostgreSQL" src="https://www.postgresql.org/media/img/about/press/elephant.png" height="70px"></a>

<a href="https://laravel.com/"><img alt="laravel" src="https://res.cloudinary.com/dtfbvvkyp/image/upload/v1566331377/laravel-logolockup-cmyk-red.svg" height="60px"></a>

<a href="https://github.com/tymondesigns/jwt-auth"><img alt="jwt-auth" src="https://cloud.githubusercontent.com/assets/1801923/9915273/119b9350-5cae-11e5-850b-c941cac60b32.png" height="70px"></a>

<a href="https://github.com/laravel/echo"><img alt="laravel-echo" src="https://laravel.com/assets/img/components/logo-echo.svg" height="50px"></a>

<a href="https://laravel.com/docs/7.x/broadcasting"><img alt="socket.io" src="https://socket.io/css/images/logo.svg" height="50px"></a>

## Use cases diagram

![Use Cases Diagram](./nbg_use_cases_diagram.svg)

## Classes diagram

![Classes Diagram](./nbg_classes_diagram.svg)

## Relations

```
1 Player        belongs to    0..N Tournament
1 Tournament    has           0..N Player

1 Player        belongs to    0..N Match
1 Match         has           2    Player

1 Player        has           0..N Map
1 Map           belongs to    1    Player

1 Player        has           0..N Shot
1 Shot          belongs to    1    Player

1 Tournament    has           0..N Match
1 Match         belongs to    0..1 Tournament

1 Match         has           2    Map
1 Map           belongs to    1    Match

1 Map           has           0..N Shot
1 Shot          belongs to    1    Map

1 Map           has           0..N Ship
1 Ship          belongs to    1    Map

1 Player        belongs to    1    GlobalRanking
1 GlobalRanking has           0..N Player
```
