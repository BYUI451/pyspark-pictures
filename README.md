# pyspark-pictures
Learn the pyspark API through pictures and simple examples

* [RDD API](pyspark-pictures.ipynb) and [PDF Slides for RDD API](visualapi.pdf)
* [DataFrame API](pyspark-pictures-dataframes.ipynb)

## RDD Example:
![example image](./images/readme-example.png)

```python
# flatMap
x = sc.parallelize([1,2,3])
y = x.flatMap(lambda x: (x, 100*x, x**2))
print(x.collect())
print(y.collect())
```
[1, 2, 3]  
[1, 100, 1, 2, 200, 4, 3, 300, 9]  


## References
[pyspark API](http://spark.apache.org/docs/latest/api/python/index.html)

## Contribute
Contributors are welcome  
Original images are [here](https://docs.google.com/presentation/d/1VFX9WMHcYiDidWdY_uYbBIFqYjG6joxN817Y6l-jD5w/edit?usp=sharing), download to pdf, convert to svg with: genSVD (pdf2svg)
