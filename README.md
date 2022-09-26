# infa_2022_khokhriakova
test test


import pygame
from pygame.draw import *

pygame.init()

FPS = 30
screen = pygame.display.set_mode((400, 400))


rect(screen, (150, 150, 250), (0, 0, 400, 200))
rect(screen, (0, 250, 0), (0, 200, 400, 200))
rect(screen, 'brown', (50, 220, 100, 100))
rect(screen, 'cyan', (85, 250, 30, 30))
polygon(screen, 'red', [(50, 220), (100,170), (150,220), (50, 220)]) 
rect(screen, (0, 0, 0, 0), (250, 150, 20, 100))
pygame.display.update()
clock = pygame.time.Clock()
finished = False

while not finished:
    clock.tick(FPS)
    for event in pygame.event.get():
        if event.type == pygame.QUIT:
            finished = True
pygame.quit()