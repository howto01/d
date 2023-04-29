# 5
df = pd.DataFrame(np.random.randn(10, 4),
index = pd.date_range('1/1/2000', periods=10), columns = ['A', 'B', 'C', 'D'])
print df
r = df.rolling(window=3,min_periods=1)
print(r.aggregate(np.sum))



# 6
pd.merge(left,right, on="id")
pd.merge(left,right, on="id", how = "left")
pd.concat(l[one, two])
one.append(two)
pd.Timestamp('2017-03-01')

#7
print pd.date_range('1/1/2011', periods=5)
print pd.date_range('1/1/2011', periods=5,freq='M')

start = pd.datetime(2011, 1, 1)
end = pd.datetime(2011, 1, 5)
print pd.date_range(start, end)
print pd.Timedelta('2 days 2 hours 15 minutes 30 seconds')
print pd.Timedelta(6,unit='h')

cat = pd.Categorical(['a', 'b', 'c', 'a', 'b', 'c'])
print df.describe()
df.plot()
df.plot.bar()
df.plot.scatter(x='a', y='b')
