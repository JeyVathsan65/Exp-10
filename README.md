import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt
df = pd.read_csv("/content/iris.csv")
df.head() dfinfo()
dfrvarietyl.value_counts()
sns.countplot(x='variety', data=df, ) plt.show() sns.scatterplot(x='sepal.length', y='sepal.width', hue='variety', data=df, )
pltlegend(bbox_to_anchor=(1, 1), loc=2) plt.show() sns.scatterplot(x='petal.length', y='petal.width', hue='variety', data=df, )
pltlegend(bbox_to_anchor=(1, 1), loc=2) plt.show() sns.pairplot(df. drop(M11, axis = 1), hue='variety', height=2) fig, axes = plt.subplots(2, 2, figsize=(10,10)) axes[0,0].set_title("Sepal Length")  
axes[0,0].hist(dff'sepallengthl, bins=7)
axes[0,1].set_title(" Sepal Width")
axes [0,1].hist(dff 'sepal.widthl , bins=5);
axes[1,0].set_title("Petal Length")
axes[1,0].hist(dfrpetallengthl, bins=6);
axes[1,1].set_title("Petal Width")
axes[1,1].hist(dff 'petal.widthl bins=6);
sns.heatmap(df.corr(method='pearson').drop(['Id'], axis=1).drop(['Id'], axis=0), annot = True);
plt.show()
