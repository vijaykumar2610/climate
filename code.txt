import matplotlib.pyplot as plt
import numpy as np

def temperature(t, a, b, c):
    return a * t ** 2 + b * t + c


a = 1
b = 2
c = 4


times = np.linspace(0, 50, 100)


temperatures = [temperature(t, a, b, c) for t in times]

plt.plot(times, temperatures)
plt.title('Temperature Model')
plt.xlabel('Time (hours)')
plt.ylabel('Temperature')
plt.grid(True)
plt.show()      

