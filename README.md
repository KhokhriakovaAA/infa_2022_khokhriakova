# infa_2022_khokhriakova
test test


import pygame 
import math
from pygame.draw import *
from math import *
pygame.init()

FPS = 30 
screen = pygame.display.set_mode((600, 400))
rect(screen, (150, 150, 250), (0, 0, 600, 200)) 
rect(screen, (0, 250, 0), (0, 200, 600, 200))


rect(screen, 'brown', (50, 220, 100, 100)) 
rect(screen, 'cyan', (85, 250, 30, 30)) 
polygon(screen, 'red', [(50, 220), (100,170), (150,220), (50, 220)])

rect(screen, 'brown', (300, 220, 80, 80)) 
rect(screen, 'cyan', (325, 245, 30, 30)) 
polygon(screen, 'red', [(300, 220), (340,170), (380,220), (300, 220)])



rect(screen, (150, 50, 50), (250, 150, 20, 100)) 
circle(screen, 'green', (250,130), 30)
circle(screen, 'green', (280,135), 30)
circle(screen, 'green', (260,115), 30)
circle(screen, 'green', (265,145), 30)
circle(screen, 'green', (280,110), 30)

rect(screen, (150, 50, 50), (450, 160, 15, 80)) 
circle(screen, 'green', (450,140), 20)
circle(screen, 'green', (480,145), 20)
circle(screen, 'green', (460,125), 20)
circle(screen, 'green', (465,155), 20)
circle(screen, 'green', (480,120), 20)


circle(screen, (255, 255, 255), (100,80), 25)
circle(screen, (255, 255, 255), (120,80), 25)
circle(screen, (255, 255, 255), (140,95), 25)
circle(screen, (255, 255, 255), (115,95), 25)
circle(screen, (255, 255, 255), (130,95), 25)
circle(screen, (255, 255, 255), (95,95), 25)
circle(screen, (255, 255, 255), (77,95), 25)

circle(screen, (255, 255, 255), (300,45), 17)
circle(screen, (255, 255, 255), (320,45), 17)
circle(screen, (255, 255, 255), (340,60), 17)
circle(screen, (255, 255, 255), (315,60), 17)
circle(screen, (255, 255, 255), (330,60), 17)
circle(screen, (255, 255, 255), (295,60), 17)
circle(screen, (255, 255, 255), (277,60), 17)

circle(screen, (255, 255, 255), (500,35), 25)
circle(screen, (255, 255, 255), (520,35), 25)
circle(screen, (255, 255, 255), (540,50), 25)
circle(screen, (255, 255, 255), (505,50), 25)
circle(screen, (255, 255, 255), (530,50), 25)
circle(screen, (255, 255, 255), (495,50), 25)
circle(screen, (255, 255, 255), (477,50), 25)


circle(screen, 'yellow', (40, 40), 20)
for i in range(50):
    polygon(screen, 'yellow', [(40-cos(360*i/50)*10,40-sin(360*i/50)*10), (40+cos(360*i/50)*10,40+sin(360*i/50)*10), (40+sin(360*i/50)*37, 40-37*cos(360*i/50)), (40-cos(360*i/50)*10,40-sin(360*i/50)*10)])






pygame.display.update() 
clock = pygame.time.Clock() 
finished = False

while not finished:
    clock.tick(FPS) 
    for event in pygame.event.get():
        if event.type == pygame.QUIT:
            finished = True 
pygame.quit()
