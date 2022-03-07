Python file
```py
from kivymd.app import MDApp
turn = 0
class Tictaktoe(MDApp):
    def __init__(self,turn=0,**kwargs):
        super().__init__(**kwargs)
        self.turn = turn
    def build(self):
        return
    def pressed1(self):

        if self.turn == 0:
            #program will run if below and will switch turns
            self.turn += 2
            # print switch to ×turn
            self.root.ids.name_label.text = "Now it is × turn"
            # change color of btn clicked
            self.root.ids.btn_1_1.text = "O"
            print(self.turn)
            self.btn_color1((0.76, 0.1, 0.1, 1))
        if self.turn == 1:
            self.root.ids.name_label.text = "Now it is ◯ turn"
            self.btn_color1((1, 0.96, 0.67, 1))
            self.root.ids.btn_1_1.text = "X"
            print(self.turn)
        self.turn-=1
    def btn_color1(self, clr):
        self.root.ids.btn_1_1.md_bg_color = clr

    def pressed2(self):

        if self.turn == 0:
            #program will run if below and will switch turns
            self.turn += 2
            # print switch to ×turn
            self.root.ids.name_label.text = "Now it is × turn"
            # change color of btn clicked
            self.root.ids.btn_1_2.text = "O"
            print(self.turn)
            self.btn_color2((0.76, 0.1, 0.1, 1))
        if self.turn == 1:
            self.root.ids.name_label.text = "Now it is ◯ turn"
            self.btn_color2((1, 0.96, 0.67, 1))
            self.root.ids.btn_1_2.text = "X"
            print(self.turn)
        self.turn-=1
    def btn_color2(self, clr):
        self.root.ids.btn_1_2.md_bg_color = clr

    def pressed3(self):

        if self.turn == 0:
            #program will run if below and will switch turns
            self.turn += 2
            # print switch to ×turn
            self.root.ids.name_label.text = "Now it is × turn"
            self.root.ids.btn_1_3.text = "O"
            # change color of btn clicked
            print(self.turn)
            self.btn_color3((0.76, 0.1, 0.1, 1))
        if self.turn == 1:
            self.root.ids.name_label.text = "Now it is ◯ turn"
            self.btn_color3((1, 0.96, 0.67, 1))
            self.root.ids.btn_1_3.text = "X"
            print(self.turn)
        self.turn-=1
    def btn_color3(self, clr):
        self.root.ids.btn_1_3.md_bg_color = clr

    def pressed4(self):

        if self.turn == 0:
            #program will run if below and will switch turns
            self.turn += 2
            # print switch to ×turn
            self.root.ids.name_label.text = "Now it is × turn"
            # change color of btn clicked
            self.root.ids.btn_2_1.text = "O"
            print(self.turn)
            self.btn_color4((0.76, 0.1, 0.1, 1))
        if self.turn == 1:
            self.root.ids.name_label.text = "Now it is ◯ turn"
            self.btn_color4((1, 0.96, 0.67, 1))
            self.root.ids.btn_2_1.text = "X"
            print(self.turn)
        self.turn-=1
    def btn_color4(self, clr):
        self.root.ids.btn_2_1.md_bg_color = clr

    def pressed5(self):

        if self.turn == 0:
            #program will run if below and will switch turns
            self.turn += 2
            # print switch to ×turn
            self.root.ids.name_label.text = "Now it is × turn"
            # change color of btn clicked
            self.root.ids.btn_2_2.text = "O"
            print(self.turn)
            self.btn_color5((0.76, 0.1, 0.1, 1))
        if self.turn == 1:
            self.root.ids.name_label.text = "Now it is ◯ turn"
            self.btn_color5((1, 0.96, 0.67, 1))
            self.root.ids.btn_2_2.text = "X"
            print(self.turn)
        self.turn-=1
    def btn_color5(self, clr):
        self.root.ids.btn_2_2.md_bg_color = clr

    def pressed6(self):

        if self.turn == 0:
            #program will run if below and will switch turns
            self.turn += 2
            # print switch to ×turn
            self.root.ids.name_label.text = "Now it is × turn"
            # change color of btn clicked
            self.root.ids.btn_2_3.text = "O"
            print(self.turn)
            self.btn_color6((0.76, 0.1, 0.1, 1))
        if self.turn == 1:
            self.root.ids.name_label.text = "Now it is ◯ turn"
            self.btn_color6((1, 0.96, 0.67, 1))
            self.root.ids.btn_2_3.text = "X"
            print(self.turn)
        self.turn-=1
    def btn_color6(self, clr):
        self.root.ids.btn_2_3.md_bg_color = clr

    def pressed7(self):

        if self.turn == 0:
            #program will run if below and will switch turns
            self.turn += 2
            # print switch to ×turn
            self.root.ids.name_label.text = "Now it is × turn"
            # change color of btn clicked
            self.root.ids.btn_3_1.text = "O"
            print(self.turn)
            self.btn_color7((0.76, 0.1, 0.1, 1))
        if self.turn == 1:
            self.root.ids.name_label.text = "Now it is ◯ turn"
            self.btn_color7((1, 0.96, 0.67, 1))
            self.root.ids.btn_3_1.text = "X"
            print(self.turn)
        self.turn-=1
    def btn_color7(self, clr):
        self.root.ids.btn_3_1.md_bg_color = clr

    def pressed8(self):

        if self.turn == 0:
            #program will run if below and will switch turns
            self.turn += 2
            # print switch to ×turn
            self.root.ids.name_label.text = "Now it is × turn"
            # change color of btn clicked
            self.root.ids.btn_3_2.text = "O"
            print(self.turn)
            self.btn_color8((0.76, 0.1, 0.1, 1))
        if self.turn == 1:
            self.root.ids.name_label.text = "Now it is ◯ turn"
            self.btn_color8((1, 0.96, 0.67, 1))
            self.root.ids.btn_3_2.text = "X"
            print(self.turn)
        self.turn-=1
    def btn_color8(self, clr):
        self.root.ids.btn_3_2.md_bg_color = clr

    def pressed9(self):

        if self.turn == 0:
            #program will run if below and will switch turns
            self.turn += 2
            # print switch to ×turn
            self.root.ids.name_label.text = "Now it is × turn"
            # change color of btn clicked
            self.root.ids.btn_3_3.text = "O"
            print(self.turn)
            self.btn_color9((0.76, 0.1, 0.1, 1))
        if self.turn == 1:
            self.root.ids.name_label.text = "Now it is ◯ turn"
            self.root.ids.btn_3_3.text = "X"
            self.btn_color9((1, 0.96, 0.67, 1))
            print(self.turn)
        self.turn-=1
    def btn_color9(self, clr):
        self.root.ids.btn_3_3.md_bg_color = clr


Tictaktoe().run()

```

kivy file
```py
MDBoxLayout:
    spacing:10
    orientation:"vertical"
    size:500,500
    size_hint:0.8,0.8
    pos_hint:{"center_x":0.5,"center_y":0.5}
    MDLabel:
        id:name_label0
        text:"Tic Tac Toe by Anju Yasu"
        size_hint:1,0.15
        font_style:"H3"
        halign:"center"
    MDLabel:
        id:name_label
        text:""
        size_hint:1,0.1
        font_style:"H4"
        halign:"center"
    MDBoxLayout:
        spacing:10
        orientation:"horizontal"
        size_hint:1,0.25
        MDRaisedButton:
            size_hint: 0.3,1
            text:" "
            id:btn_1_1
            font_style:"H4"
            md_bg_color:0.6,0.9,0.83,1
            on_release:
                app.pressed1()
        MDRaisedButton:
            size_hint: 0.3,1
            text:" "
            id:btn_1_2
            font_style:"H4"
            md_bg_color:0.6,0.9,0.83,1
            on_release:
                app.pressed2()
        MDRaisedButton:
            size_hint: 0.3,1
            text:" "
            id:btn_1_3
            font_style:"H4"
            md_bg_color:0.6,0.9,0.83,1
            on_release:
                app.pressed3()
    MDBoxLayout:
        spacing:10
        orientation:"horizontal"
        size_hint:1,0.25
        MDRaisedButton:
            size_hint: 0.3,1
            text:" "
            id:btn_2_1
            font_style:"H4"
            md_bg_color:0.6,0.9,0.83,1
            on_release:
                app.pressed4()
        MDRaisedButton:
            size_hint: 0.3,1
            text:" "
            id:btn_2_2
            font_style:"H4"
            md_bg_color:0.6,0.9,0.83,1
            on_release:
                app.pressed5()
        MDRaisedButton:
            size_hint: 0.3,1
            text:" "
            id:btn_2_3
            font_style:"H4"
            md_bg_color:0.6,0.9,0.83,1
            on_release:
                app.pressed6()
    MDBoxLayout:
        spacing:10
        orientation:"horizontal"
        size_hint:1,0.25
        MDRaisedButton:
            size_hint: 0.3,1
            text:" "
            id:btn_3_1
            font_style:"H4"
            md_bg_color:0.6,0.9,0.83,1
            on_release:
                app.pressed7()
        MDRaisedButton:
            size_hint: 0.3,1
            text:" "
            id:btn_3_2
            font_style:"H4"
            md_bg_color:0.6,0.9,0.83,1
            on_release:
                app.pressed8()
        MDRaisedButton:
            size_hint: 0.3,1
            text:" "
            id:btn_3_3
            font_style:"H4"
            md_bg_color:0.6,0.9,0.83,1
            on_release:
                app.pressed9()
```
<img width="807" alt="Screenshot 2022-03-08 at 0 20 10" src="https://user-images.githubusercontent.com/89366347/157062796-60623e91-cba7-42e9-9fe6-46502409815a.png">

