# ball
import math

# Размеры бассейна в метрах
length = 10
width = 10
height = 1  # Предположим, что высота слоя шариков 1 метр

# Диаметр одного шарика в метрах
ball_diameter = 0.1  # Например, 10 см

# Рассчитываем объем бассейна
pool_volume = length * width * height

# Рассчитываем объем одного шарика
ball_radius = ball_diameter / 2
ball_volume = (4/3) * math.pi * ball_radius**3

# Рассчитываем количество шариков, которые могут поместиться в бассейн
number_of_balls = pool_volume // ball_volume  # Используем целочисленное деление для получения целого числа

print(f"Примерное количество шариков, которые могут поместиться в бассейн: {number_of_balls}")
