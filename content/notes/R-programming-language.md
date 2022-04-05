---
title: R Programming Language
disableToc: true
---

### R Programming Language
Programming language used for the analysis and visualization of data.

#### Data Types
| Type      | Example |
| --------- | ------- |
| Integer   | 1       |
| Numeric   | 1.3     |
| Character | "One"   |
| Factor    | One     |
| Logical   | TRUE    |
| NA        | NA      |
| Null      | null    |

#### Vectors
To create a [[notes/vector]]:
`myVector = c(1,2,3,4)`
Vectors are created with the `c()` function, and can only contain a single data type. Vectors work similarly to dictionaries in python.

To add an element to a vector, we also use the `c()` function.
```
myVector = c(myVector, 5)

myVector
[1] 1 2 3 4 5
```

Vectors start at $1$.

#### Matrices
[[notes/matrix|Multidimensional]] vector. Can also only contain single data types.
`myMatrix = matrix(1:12, nrow=3, ncol=4)`
This creates a $3\times4$ matrix with values from $1$ to $12$. 

#### Data Frame
A data frame is a specific type of matrix, where each column can have its own data type.

#### Downloading Files
To download files directly from the internet:
```
download.file(
	url = "https://archive.ics.uci.edu/ml/machine-leanning-databases/iris/iris.data"
	destfile = "iris.data"
)
```
Where `url` is the location of the file and `destfile` is the destination file.

#### Graphs
We use different functions depending on the type of plot we want to make:
- `plot()`
- `hist()`
- `barplot()`
- `boxplot()`

#### Functions
```
sum<-function(x,y){
	# Add elements x and y
	x+y
}

sum(4,5)
```


#programming #R
