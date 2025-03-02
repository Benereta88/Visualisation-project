# Visualisation-project

# Spider hart
import matplotlib.pyplot as plt
import numpy as np
import seaborn as sns


labels = np.array([ "A", "B", "C", "D", "E", "F"])
data = np.array([4, 5, 2, 5, 3, 5])


sns.set_theme(style="dark")
sns.set_palette("muted")

angles = np.linspace(0, 2 * np.pi, len(labels), endpoint=False)
data = np.concatenate((data, [data[0]]))
angles = np.concatenate((angles, [angles[0]]))

plt.polar(angles, data, marker="o")
plt.fill(angles, data, alpha=0.25)
plt.title("Spider chart")
plt.show()



# Violin plot
import seaborn as sns
import matplotlib.pyplot as plt
import numpy as np


sns.set_theme(style="dark")
sns.set_palette("muted")

data = [np.random.normal(0, std, 100) for std in range(1, 4)]

sns.violinplot(data=data)
plt.title("Violin plot")
plt.xlabel("Category")
plt.ylabel("Values")
plt.show()

# Box plot 
import seaborn as sns
import matplotlib.pyplot as plt
import numpy as np

data = [ np.random.normal(0, std, 100) for std in range(1, 4)]

sns.boxplot(data=data)
plt.title("Box plot")
plt.xlabel("Category")
plt.ylabel("Values")
plt.show()

# Area chart
import matplotlib.pyplot as plt

x = [1, 2, 3, 4, 5]
y1 = [30, 20, 30, 20, 30]
y2 = [25, 10, 25, 10, 25]

plt.fill_between(x, y1, y2, color="skyblue", alpha=1)
plt.title("Area chart")
plt.xlabel("x-axis")
plt.ylabel("y-axis")
plt.show()

# Cyrkel chart

import matplotlib.pyplot as plt

labels = ["Category A", "Category B", "Category C"]
sizes = [10, 65, 25 ]
explode = (0.5, 0.5, 0.5)
print(len)


plt.pie(sizes, labels=labels, autopct= "%1.1f%%")
plt.title("Pie chart")
plt.show()

# Bar chart

import seaborn as sns
import matplotlib.pyplot as plt
import numpy as np

categories = ["A", "B", "C", "D"]
values = [25, 40, 30, 20]

sns.set_theme(style="dark")
sns.set_palette("muted")

plt.bar(categories, values)
plt.title("Bar chart")
plt.xlabel("Categories")
plt.ylabel("Values")
plt.show()

