from tkinter import Tk, Canvas
from tkinter import *
from tkinter import ttk

# Создаем главное окно
root = Tk()
root.title("Домик")
btn = ttk.Button(text="Вкл, выкл.)
btn.pack()


# Создаем холст для рисования
canvas = Canvas(root, width=400, height=300)
canvas.pack()

# Функция для рисования домика
def draw_house(canvas):
    # Основание дома
    canvas.create_rectangle(110, 300, 290, 160, fill="brown")

    # Крыша дома
    canvas.create_polygon(100, 160, 200, 0, 300, 160, fill="green")

    # Окна
    canvas.create_rectangle(160, 260, 250, 190, fill="white")

# Вызываем функцию для рисования домика
draw_house(canvas)

# Запускаем главный цикл обработки событий
root.mainloop()
160, 250, 240, 190
