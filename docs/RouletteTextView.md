---
layout: default
title: RouletteTextView
---

# [RouletteTextView](https://github.com/DarkTornado/RouletteTextView)
public class RouletteTextView extends WebView

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

## void setGravity(int gravity);
* Set texts' gravity in `RouletteTextView`.

## void setMovingData(int delay, int distance, int range);
* Set texts' attribute in `RouletteTextView`.
* Texts in `RouletteTextView` will move `distance` pixels every `delay` second.
* Texts will move between `-range` and `range` pixels.

## void setSize(int width, int height);
* Set `RouletteTextView`'s size.

## void setTexts(String[] data);
* Set texts that will be showed in `RouletteTextView`.

## void setTexts(List<String> data);
* Set texts that will be showed in `RouletteTextView`.

## void setTextColor(int color);
* Set text's color in `RouletteTextView`.

## void setTextSize(int px);
* Set text's size in `RouletteTextView`.

## void stop();
* Makes texts in `RouletteTextView` stop.