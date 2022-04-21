---
layout: default
title: AlertWindow
---

# [AlertWindow](https://github.com/DarkTornado/AlertWindow)
public class AlertWindow extends java.lang.Object

* What made with `WindowManager`, which can be used as `AlertDialog`.
* You can use `AlertWindow` in `Service` because it is made with `WindowManager`.
* 다이얼로그랑 비슷한 역할을 하는 `WindowManager`로 구현된 것.
* `WindowManager`로 구현되어 있기 때문에, `Service`에서도 사용 가능

***

# Constructor / 생성자

## AlertWindow(Context ctx);
* `ctx` is Context of application.
* `ctx`는 애플리케이션의 Context.

## AlertWindow(Context ctx, boolean hasEditText);
* If you want to input value to `EditText` in `AlertWindow`, you should set `hasEditText` as `true`.
* If `hasEditText` is true, you cannot touch `AlertWindow`'s outside, but, you can touch when it is foldeded.
* `AlertWindow` 안에 있는 `EditText`에 값을 입력하고 싶다면, `hasEditText`를 `true`로 설정해야 해요.
* `hasEditText`가 `true`라면 `AlertWindow`의 밖을 터치할 수 없지만, 접은 상태에서는 터치할 수 있어요.

***

# Method / 메서드

## void close();
* Dismiss the `AlertWindow`.
* `AlertWindow` 삭제.

## void useCloseButton(boolean use);
* Select using `X Bbutton` or not. Defualt is `true`.
* `X버튼`을 사용할지 말지 결정해요. 기본값은 `true`.

## void setDraggable(boolean canDrag);
* If `canDrag` is `true`, you can change the `AlertWindow`'s position by dragging its title. Defualt is `true`.
* `AlertWindow`의 타이틀 부분을 길게 눌러서 위치를 바꿀 수 있도록 할지 설정해요. 기본값은 `true`.

## void setFoldable(boolean canFold);
* If `canFold` is `true`, you can fold the `AlertWindow` by touching its title. Defualt is `false`.
* `AlertWindow`의 타이틀 부분을 길게 눌러서 접을 수 있도록 할지 설정해요. 기본값은 `false`.

## void setMessage(String msg);
* Set `AlertWindow`'s message.
* `AlertWindow`에 담길 메시지를 설정해요.

## void setTitle(String title);
* Set `AlertWindow`'s title.
* `AlertWindow`의 타이틀을 설정해요.

## void setView(View view);
* Set `AlertWindow`'s view. I recommend using `LinearLayout` as a parameter.
* `AlertWindow`의 뷰 설정해요. `LinearLayout`을 매개변수로 사용하는 것을 추천합니담.

## void setButton(String txt, View.OnClickListener listener);
* Set Button to `AlertWindow` likes `AlertDialog`'s `NegativeButton`.
* `AlertDialog`에 있는 `부정 버튼`과 같은 버튼을 `AlertWindow`에 설정해요.

## void show();
* Show the `AlertWindow` on display.
* 화면에 `AlertWindow`를 출력해요

