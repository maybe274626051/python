# python
import random
boxs = [[], [], []]
redball = ["r", "r", "r"]
bullball = ["b", "b", "b"]
whiteball = ["w", "w", "w", "w"]

for box in boxs:
    box.append(whiteball.pop())
balls = redball + bullball + whiteball
for ball in balls:
    boxs_index = random.randint(0,len(boxs)-1)
    boxs[boxs_index].append(ball)
print(boxs)
