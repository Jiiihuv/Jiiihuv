@@ -107,6 +107,19 @@ If you want to make many apperances of `idx=2`, you can write them repeatedly. (
![header](https://capsule-render.vercel.app/api?color=gradient&customColorList=0,2,2,5,30)
```

## Theme
You can use the specified combination using `theme=`.

Even if `color` and `fontColor` are used, theme has the highest priority.

Check the list of available themes at [pallete_theme.json](https://github.com/kyechan99/capsule-render/blob/master/src/pallete_theme.json).

```
![reversal](https://capsule-render.vercel.app/api?type=rect&text=RECT&fontAlign=30&fontSize=30&desc=Use%20theme&descAlign=60&descAlignY=50&theme=radical)
```

> I'm currently adding combinations from the [Link:theme](https://github.com/anuraghazra/github-readme-stats/blob/master/themes/README.md) little by little.
## Section
Section data makes reverse Background Image.
- `&section=header` : (default)
- `&section=footer`
Write `&section= ` on the URL
```
![footer](https://capsule-render.vercel.app/api?section=footer)
```
## Reversal
Reverse the image left and right. (Color at the same time)
- `&reversal=false` : (default)
- `&reversal=true`
```
![reversal](https://capsule-render.vercel.app/api?type=slice&reversal=true&color=gradient)
```
## Height
Change Image Size. Default value is 120.
Write `&height= ` on the URL
```
![header](https://capsule-render.vercel.app/api?height=400)
```
> Do not write `px`
## Text
Input text over the Image.
Write Something `&text= `.
```
![header](https://capsule-render.vercel.app/api?text=Hello%World!)
```
> You can't use some Special Characters. Like '#', '&', '/' ... 
>
> It makes confused API
> It is recommended to use `%20` (blank) only
## Desc
Input desc over the Image.
Write Something `&desc= `.
```
![header](https://capsule-render.vercel.app/api?height=400&text=Hello%20World!&desc=Hello%20capsule%20render)
```
> You can't use some Special Characters. Like '#', '&', '/' ... 
>
> It makes confused API
> It is recommended to use `%20` (blank) only
## Text Background
Background of Text.
Write `&textBg=true` to active.
> If you want to increase background-size, 
add `%20` between text values.
This is because background-size depends on the length of the english-text. (%20 means spacing)
```
![header](https://capsule-render.vercel.app/api?type=rounded&color=gradient&text=%20asdf%20&height=300&fontSize=100&textBg=true)
```
## Text Animation
Make the text dynamic.
Write `&animation= `, if you want to use.
- `fadeIn` : fadeIn 1.2s
- `scaleIn` : scaleIn .8s
- `blink` : blink .6s
- `blinking` : blinking 1.6s
- `twinkling` : twinkling 4s
```
![header](https://capsule-render.vercel.app/api?text=capsule_render&animation=fadeIn)
```
## FontColor
Change text color. Default value is 000000.
Value should be Hex code with erased '#'
Write `&fontColor= ` behind **Text** query
```
![header](https://capsule-render.vercel.app/api?text=Hello%World!&fontColor=d6ace6)
```
## FontSize
Change text font size. Default value is 70.
Write `&fontSize= ` behind **Text** query
```
![header](https://capsule-render.vercel.app/api?text=Hello%World!&fontSize=40)
```
> Do not write `px`
## FontAlign
Change text horizontal-align (x). write number **between 0~100**
`&fontAlign= ` : Default value is 50. center of image
```
![header](https://capsule-render.vercel.app/api?text=Hello%World!&fontAlign=70)
```
## FontAlignY
Change text vertical-align (y). write number **between 0~100**
`&fontAlignY= ` : Default value is 50. center of image
```
![header](https://capsule-render.vercel.app/api?text=Hello%World!&fontAlignY=20)
```
## DescSize
Change desc font size. Default value is 20.
Write `&descSize= ` behind **desc** query
```
![header](https://capsule-render.vercel.app/api?text=Hello%World!&fontSize=40&desc=Desc&descSize=30)
```
> Do not write `px`
## DescAlign
Change desc horizontal-align (x). write number **between 0~100**
`&descAlign= ` : Default value is 50. center of image
```
![header](https://capsule-render.vercel.app/api?text=Hello%World!&fontAlign=70&desc=Desc&descAlign=20)
```
## DescAlignY
Change text vertical-align (y). write number **between 0~100**
`&descAlignY= ` : Default value is 60. center of image
```
![header](https://capsule-render.vercel.app/api?text=Hello%World!&fontAlignY=20&desc=Desc&descAlignY=40)
```
## Rotate
Usage `&rotate= `, to rotate text.
You can also use negative number.
> Recommend number arrange. ☞ `0 ~ 360`, `0 ~ -360`. 
```
![header](https://capsule-render.vercel.app/api?text=Hello%World!&fontSize=20&rotate=-30)
```
## Stroke
Change text stroke.
Write `&stroke=` behind query
Value should be Hex code with erased '#'
```
![header](https://capsule-render.vercel.app/api?type=rect&height=200&text=Stroke%20Test&fontAlign=70&stroke=00FF00)
```
> Recommended to use with `strokeWidth`.
>
> When used alone, strokeWidth defaults to 1.
## Stroke-width
Change text stroke width.
Write `&strokeWidth=` behind stroke query
Value must be greater than or equal to 0.
```
![header](https://capsule-render.vercel.app/api?type=rect&height=200&text=Stroke%20Test&fontAlign=70&stroke=00FF00&strokeWidth=3)
```
> Recommended to use with `stroke`.
>
> When used alone, stroke defaults to 'B897FF'.
# Demo <a id="demo">
## Wave <a id="wave">
![wave](https://capsule-render.vercel.app/api?type=wave&color=auto&height=200&text=WAVE)
## Egg <a id="egg">
![egg](https://capsule-render.vercel.app/api?type=egg&color=auto&height=210)
## Shark <a id="shark">
![shark](https://capsule-render.vercel.app/api?type=shark&color=gradient&height=140)
## Slice <a id="slice">
![slice](https://capsule-render.vercel.app/api?type=slice&color=auto&height=200&text=SLICE&fontAlign=70&rotate=13&fontAlignY=25&desc=desc%20function%20is%20also%20rotated.&descAlign=70.&descAlignY=44)
  
## Rect <a id="rect">
![rect](https://capsule-render.vercel.app/api?type=rect&color=gradient&text=%20%20RECT%20%20&fontAlign=30&fontSize=30&textBg=true&desc=Use%20%27textBg%27%20to%20highlight%20%27text%27&descAlign=60&descAlignY=50)
## Soft <a id="soft">
![soft](https://capsule-render.vercel.app/api?type=soft&color=auto&text=Good%20to%20use%20with%20other%20readme&fontSize=40&animation=twinkling)
## Rounded <a id="rounded">
![rounded](https://capsule-render.vercel.app/api?type=rounded&color=timeAuto&text=Rounded%20with%20stroke&fontAlignY=50&fontSize=40&height=200&stroke=000000&strokeWidth=2)
## Cylinder <a id="cylinder">
![cylinder](https://capsule-render.vercel.app/api?type=cylinder&color=auto&text=Cylinder&fontAlignY=45&fontSize=40&height=150&animation=blinking&desc=desc%20is%20also%20animated&descAlignY=70)
## Waving <a id="waving">
![waving](https://capsule-render.vercel.app/api?type=waving&height=200&text=Waving!&fontAlign=80&fontAlignY=40&color=gradient)
## Transparent <a id="transparent">
![transparent](https://capsule-render.vercel.app/api?type=transparent&fontColor=703ee5&text=Transparent&height=150&fontSize=60&desc=Only%20Use%20Text&descAlignY=75&descAlign=60)
<hr/>
# Things that helped contribute
- SVG Path Easy Maker [Codepen](https://codepen.io/kyechan99/pen/yLeQVBa)
- SVG Path draw [mavo.io](https://mavo.io/demos/svgpath/)
![footer](https://capsule-render.vercel.app/api?type=wave&color=auto&height=200&section=footer&text=Now%20Use%20me!&fontSize=90)


# - 이름:탁강현
## - 나이:26세(만25세)
### - 출신:포항
### - 학력: 창원기계공업고등학교(졸업),창원폴리텍대학교(재학)
#### - 자격증: 전기기능사


<h3 align="center">👩‍💻 My Github Stats 👩‍💻</h3>
<div align="center">

[![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=hyeinisfree&hide_title=true&show_icons=true&include_all_commits=true&disable_animations=true&theme=vue)](https://github.com/anuraghazra/github-readme-stats)
</div>

<p align="center">
  <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fhyeinisfree&count_bg=%2341B883&title_bg=%23CDC2C2&icon=github.svg&icon_color=%23E7E7E7&title=hits&edge_flat=false"/></a>
</p>

<h3 align="center">📚 Tech Stack 📚</h3>
<p align="center">
  <img src="https://img.shields.io/badge/Java-007396?style=flat-square&logo=Java&logoColor=white"/></a>&nbsp
  <img src="https://img.shields.io/badge/Python-3766AB?style=flat-square&logo=Python&logoColor=white"/></a>&nbsp 
  <img src="https://img.shields.io/badge/Javascript-ffb13b?style=flat-square&logo=javascript&logoColor=white"/></a>&nbsp 
  <br>
  <img src="https://img.shields.io/badge/Spring-6DB33F?style=flat-square&logo=Spring&logoColor=white"/></a>&nbsp
  <img src="https://img.shields.io/badge/SpringBoot-6DB33F?style=flat-square&logo=SpringBoot&logoColor=white"/></a>&nbsp 
  <img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=Node.js&logoColor=white"/></a>&nbsp
  <img src="https://img.shields.io/badge/Express-000000?style=flat-square&logo=Express&logoColor=white"/></a>&nbsp
  <br>
  <img src="https://img.shields.io/badge/Mysql-E6B91E?style=flat-square&logo=MySql&logoColor=white"/></a>&nbsp 
  <img src="https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=AmazonAWS&logoColor=white"/></a>&nbsp 
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=Docker&logoColor=white"/></a>&nbsp 
  <img src="https://img.shields.io/badge/Jenkins-D24939?style=flat-square&logo=Jenkins&logoColor=white"/></a>&nbsp 
</p>

<h3 align="center">🌈 Follow Me 🌈</h3>
<p align="center">
  <a href="t01091020385@gmail.com"><img src="https://img.shields.io/badge/Gmail-d14836?style=flat-square&logo=Gmail&logoColor=white&link=kimhyein7110@gmail.com"/></a>
</p>

# - 자기소개서
### - 안녕하세요 저는 창원에 살고있는 탁강현입니다. 
 저는 2남중 장남으로 포항에 태어나 포항에서 어린시절을 보내다가 고등학교때 창원으로 와서
 창원기계공업고등학교에 디지털 전기과를 나왔습니다. 고등학교 3학년때 아림지앤코라는 회사에 취업을하여
 특례를 하고 3년동안 다니다 회사가 망하여 그만두게 되었습니다. 그리고 다시 다른 회사에 취업을 하여 2년 6개월동안 일을하다가
 삼성전기에 지원을하여 최종면접에서 떨어지고 갑자기 공부를 하고싶다는 생각이 들어서 폴리텍대학교 스마트팩토리과에 지원을 하여서
 2022년도에 폴리텍을 오게 되었습니다. 스마트팩토리과를 설명을 좀 드리자면 제품을 조립,포장하고 기계를 점검하는 전 과정이 자동으로
 이뤄지는 공장으로 정보통신기술(ICT)의 융합으로 이뤄지는 차세대 산업혁명인 4차 산업혁명의 핵심으로 꼽힙니다. 
 스마트팩토리는 모든 설비와 장치가 무선통신으로 연결되어 있기 때문에 실시간으로 전 공정을 모니터링하고 분석할 수 있습니다.
 스마트 팩토리에서는 공장 곳곳에 사물인터넷(IoT) 센서와 카메라를 부착시켜 데이터를 수집하고 플랫폼에 저장해 분석하는데,
 이렇게 분석된 데이터를 기반으로 어디서 불량품이 발생하였는지, 이상 징후가 보이는 설비는 어떤 것인지 등을 인공지능이 파악하여 전체적인 공정을 제어합니다.
 제가 가고싶은 꿈의 회사는 Sk하이닉스와 삼성전기 그리고 볼보 입니다. 제가 취득하고싶은 자격증은 전기기사와 기계정비산업기사 생산자동화산업기사 입니다.
 그리고 제가 얼마전에 지게차기능사 필기에 합격을하여 실기를 준비중입니다.

## - 아래의 표는 제가 파이썬을 공부하고 만들어본 표입니다

|함수|함수|함수|함수|
|-----|-----|-----|-----|
|int|float|complxe|str|
|repr|eval|tuple|list|
|set|dict|frozenset|chr|
|unichr|ord|hex|oct|

<!---
Jiiihuv/Jiiihuv is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
