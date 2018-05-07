## 3(a)
```py
pts = np.array([(3,6),(6,4),(4,7),(7,2),(3,4),(-1,7),(-3,2)])

```
## (i)
```py
pts[:,0] # [3,6,4,7,3,-1,-3]
plt.plot(pts[:,0])
```
![image](https://user-images.githubusercontent.com/23183656/39692400-563b08c6-5213-11e8-8b86-8d4f45805a62.png)

## (ii)
```py
plt.scatter(pts[:,0], pts[:,1])
# pts[:,0] => [3,6,4,7,3,-1,-3]
# pts[:,1] => [6,4,7,2,4, 7,2]
```
![image](https://user-images.githubusercontent.com/23183656/39692637-fbc43272-5213-11e8-9bc9-01f1552b4214.png)

## (iii)
```py
plt.hist(pts[:,1])
# pts[:,1] => [6,4,7,2,4,7,2]
```
The histogram is plotted based on frequency.
![image](https://user-images.githubusercontent.com/23183656/39692833-a8c68204-5214-11e8-9615-3270a9b8707c.png)




