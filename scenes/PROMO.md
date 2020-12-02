# intro

`SceneSetup.intro();`

# intro-play-button

(...51)

[CHƠI!](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

# intro-start

(...500)

`clearText()`

n3: Vậy trước khi chúng ta bắt đầu, * bạn * muốn đọc như thế nào?

`publish("show_options_bottom")`

# intro-start-2

n3: Bây giờ, hãy bắt đầu câu chuyện của chúng ta ...

```
publish("hide_tabs");
clearText();
```

(...1000)

`publish("intro-to-game-2")`

n2: THIS IS A HUMAN

(...600)

`clearText()`

(...300)

`publish("intro-to-game-3")`

# act1

```
SceneSetup.act1();
publish("hide_tabs");
music('battle', {volume:0.5});
```

(...300)

n: VÀ ĐÂY LÀ SỰ LO NGẠI CỦA CON NGƯỜI

n: _BẠN_ LÀ SỰ LO NGẠI

(#act1_normal)


# act1_normal

```
hong({body:"putaway"});
sfx("rustle");
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Không. Không, không, không nghe. Sẽ kiểm tra điện thoại của tôi.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: CÔNG VIỆC CỦA BẠN LÀ BẢO VỆ CON NGƯỜI CỦA BẠN KHỎI * NGUY HIỂM *

`bb({eyes:"look", mouth:"small_lock", body:"fear"})`

b: Thở hổn hển! Bạn đang cuộn cuộc sống của mình trên Twitter! Lần nữa!

```
bb({eyes:"normal", mouth:"normal", body:"normal"});
hong({eyes:"annoyed"});
```

h: Yeah Tôi tự hỏi tại sao tôi không chỉ ngồi và lắng nghe những suy nghĩ của tôi thường xuyên hơn.

`hong({eyes:"neutral"});`

n: NHANH CHÓNG, CẢNH BÁO HỌ VỀ *NGUY HIỂM!*

```
bb({eyes:"look"});
```

[Ồ không, hãy xem câu chuyện thời sự kinh khủng đó!](#act1d_news)

[Ồ không, tweet đó có phải là bí mật về * chúng tôi không? *](#act1d_subtweet)

[Này, GIF mèo đang uống sữa](#act1d_milk)

# act1d_milk

`hong({mouth:"smile", eyes:"surprise"});`

h: Heh ya thật dễ thương, tôi--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: MÈO KHÔNG THỂ TIÊU HÓA SỮA VÀ CHÚNG TÔI LÀ NHỮNG NGƯỜI KHỦNG KHIẾP ĐỂ THƯỞNG THỨC LỢI NHUẬN CỦA ĐỘNG VẬT

(...200)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("20p", "bad");
publish("hp_show");
```



