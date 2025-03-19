import numpy as np
import matplotlib.pyplot as plt
import math

# calculate the upper bound value of log2 of n
def upper_value_log2(n):
    return math.ceil(math.log2(n)) if n > 1 else 1

n_values = np.arange(2, 1000)

# calculating the functions
n_graph = n_values
sqrt_n_log_graph = np.sqrt(n_values) * np.array([upper_value_log2(n) for n in n_values])

# drawing the graphs
plt.figure(figsize=(10, 6))
plt.plot(n_values, n_graph, label='n', color='blue')
plt.plot(n_values, sqrt_n_log_graph, label=r'$\sqrt{n} \cdot \lceil \log_2 n \rceil$', color='red')

# putting labels and titles for easy reading
plt.xlabel('n')
plt.ylabel('Function Values')
plt.title(r'$\lceil n \rceil$ and $\sqrt{n} \cdot \lceil \log_2 n \rceil$')
plt.legend()
plt.grid()
plt.savefig("plot_eval.png")
