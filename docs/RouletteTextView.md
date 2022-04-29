---
layout: default
title: RouletteTextView
---

# [RouletteTextView](https://github.com/DarkTornado/RouletteTextView)
public class RouletteTextView extends android.webkit.WebView

* A `View` which contains text that rotates like a slot machine.
* 슬롯머신 비슷하게 위에서 아래로 돌아가는 텍스트를 포함하고 있는 `View`.

***

# Constructor / 생성자

## RouletteTextView(Context context);
* `ctx` is Context of application.
* `ctx`는 애플리케이션의 Context.

***

# Method / 메서드

## void create();
* Create internal part of `RouletteTextView`.
* You should call this method before you put `RouletteTextView` to another view.
* `RouletteTextView`의 내부 부분을 구현시키는 메서드로, 다른 뷰에 넣기 전에 호출해야 해요.

## void setBackgroundColor(int color);
* Set `RouletteTextView`'s background color.
* `RouletteTextView`의 배경색 설정

## void setGravity(int gravity);
* Set texts' gravity in `RouletteTextView`.
* `RouletteTextView`의 정렬 방향 설정

## void setMovingData(int delay, int distance, int range);
* Set texts' attribute in `RouletteTextView`.
* Texts in `RouletteTextView` will move `distance` pixels every `delay` second.
* Texts will move between `-range` and `range` pixels.
* `RouletteTextView` 안에 들어가는 문구들이 `delay`초마다 `distance` 픽셀 씩 이동하게 설정해요.
* 해당 문구는 `-range` 필셀부터 `range` 픽셀 사이 영역에서 움직일거에요.

## void setSize(int width, int height);
* Set `RouletteTextView`'s size.
* `RouletteTextView`의 크기 설정

## void setTexts(String[] data);
* Set texts that will be showed in `RouletteTextView`.
* `RouletteTextView`에 들어갈 문구들 설정

## void setTexts(List&lt;String&gt; data);
* Set texts that will be showed in `RouletteTextView`
* `RouletteTextView`에 들어갈 문구들 설정

## void setTextColor(int color);
* Set text's color in `RouletteTextView`.
* `RouletteTextView`에 들어갈 문구의 색상 설정

## void setTextSize(int px);
* Set text's size in `RouletteTextView`.
* `RouletteTextView`에 들어갈 문구의 크기 설정

## void stop();
* Makes texts in `RouletteTextView` stop.
* `RouletteTextView`에서 돌아가고 있는 문구들이 멈추게 설정
