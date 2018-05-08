## (i)
- CSV stands for Comma Separated Value
- It is like a table
- Usually the first line will be the headings
- Each line represent one record
- Example:
```
Name,Age,Hobby
"Ali",12,"ping pong"
"Abu",99,"badminton"
"Johny",122,"dota"
```

## (ii)
Advantages of CSV:
- Quite compact (smaller file size) when compared to JSON and XML
- Faster to process than other format


## (iii)
Disadvantages of CSV:
- CSV has poor support for special characters 
- No easy distinction between text and numerical value
- It is not self-describing 
- Quite hard to store nested or unstructured/schema-less data (although it is possible)
- Lack of universal standards

## (iv)
JSON. JSON is self-describing and also have good support for nested and schema-less data.

For example, I can have the following data in JSON :
```js
[{
    name: "John",
    age: 12,
    friends: [
        {
            name: "Chan",
            age: 99,
        }, {
            name: "Lee",
            age: 12
        }
    ]
}]
```
This type of data can be easily represented using JSON, however it is hard store it in CSV format, because CSV expect flat data.  

Anyway, it is possible to store the data above in CSV, one of the solution is to embed the JSON into it.

```
name,age,friends
"John",12,"[{name:\"Chan\",age:99},{name:\"Lee\",age:12}]"

```
Yea, it looks disgusting, but in reality most of the data looks exactly like this, or even more disgusting (*it's not rare that you will have more than 100 columns and few million rows of data!*).

That's why Dr. Tay says that *data scientists* are like *janitor*, because they spend most of the time cleaning data.