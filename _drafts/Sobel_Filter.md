---
title: Sobel-Feldman Operator / Sobel Filter
author: Jang_Hyeoon_Soo
date: 2020-08-30
categories: [knowledge, filter]
tags: [Sobel_filter, Sobel_Operator, filter, Sobel]
pin: true
use_math: true
---

# 사용 용도

- 영상 처리 시 윤곽선, 경계선을 강화하는 효과가 있음


# 원리
일반적으로 영상 데이터는 벡터, 행렬로 표현한다. 경계선에 가까운 특수한 경우를 제외한다면 영상의 임의의 지점과 그 주변은 다음과 같이 보일 것이다.

![3x3_Matrix_General](https://user-images.githubusercontent.com/48907725/91654809-fc084700-eae6-11ea-8e70-bb11486a93c0.JPG)

가운데인 e점을 기준으로 주변 값이 얼마나 차이가 나는지 구한다. 차이가 많이 난다는 것은 영상에서 경계선을 의미한다. 그래서 원본 영상에서 주변 값 차이가 많이 나는 지점은 그 차이를 더 강화하면 경계선이 더 선명해지는 효과를 얻을 수 있다.

먼저 e점을 기준으로 gradient를 구한다면 이것은 변화량/거리로 표현할 수 있다. 수평, 수직으로 한 칸 움직이는 것을 거리가 1이라고 하면 인접한 대각선은 거리가 2가 된다. 수식은 다음과 같다.
    
$
G = (c-g)/4 * [1, 1] + 
    (a-i)/4 * [-1, 1] + 
    (b-h)/2 * [0, 1] + 
    (f-d)/2 * [1, 0] 
$
    
결국 다음과 같은 결과를 얻는다.

$ G' = 4G = [c-g-a+i + 2(f-d), c-g+a=i + 2*(b-h)] $

또는 기본적인 gradient 연산을 이용한 접근법도 있다. 영상의 기울기를 얻으려면 모든 화소 위치에서 편미분 \deltaf/\deltay를 계산해야 한다.
    

$g_x = \frac {$\delta$f(x,y)}{\deltax} = f(x+1, y) - f(x, y)$
$g_y = \frac ${\delta$f(x,y)}{\deltay} = f(x, y+1) - f(x, y)$


크기를 3x3으로 확장하고 가장 단단한 경우를 보면 다음과 같을 것이다.    
    
$
g_x = \frac {\delta f}{\delta x} = (g + h + i) - (a + b + c)   
g_y = \frac {\delta f}{\delta y} = (c + f + i) - (a + d + g)
$

결국 다음과 같은 마스크를 얻을 수 있다.    

<img style="float: left;" src="https://user-images.githubusercontent.com/48907725/91657775-988a1380-eafe-11ea-92c8-3514bc095723.JPG">
<img style="float: center;" src="https://user-images.githubusercontent.com/48907725/91657776-9fb12180-eafe-11ea-8cad-8663f9ca8f2f.JPG">

같은 원리로 대각선 Sobel Operator를 만들 수 있다.

![3x3_Matrix_General](https://user-images.githubusercontent.com/48907725/91657768-88723400-eafe-11ea-910a-271a0473b2e3.JPG)


# 소스코드


# 참고자료
[Isotropic 3x3 Image Gradient Operator](https://www.researchgate.net/publication/239398674_An_Isotropic_3x3_Image_Gradient_Operator)     
Digital Image Processing, Rafael C. Gonzalez, Richard E. Woods, PEARSON    
