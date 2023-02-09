# JASON 101
![JSON](images/json.webp)

## JavaScript Object Notation
Is a lightweight data-interchange format. It's easy for `humans` to read and write. It's easy for `machines` to parse and generate.

## Introduction
An `object` is an unordered set of `key:value` pairs enclosed by `{ }`.
```js
{"physical": "layer1", "data link": "layer2"}
```
An `array` is an ordered collection of `values`, sperated by commas and encluded in `[ ]`.
```js
["physical", "data link", "network"]
```

`Values` can be a string, object, number, array, true, false and null.

# Sample JSON Document
Sample Document
```JS
{
  "names": ["physical", "data link", "network"],
  "layers": ["layer 1", "layer 2", "layer 3"]
}
```
Sample Top Level Document
```js
{
    "physical" : {
        "layer": 1,
        "description": "something"
    },
    "data" : {
        "layer": 2,
        "description": "something"
    },
    "network" : {
        "layer": 3,
        "description": "something"
    }
}
```
# Sample CloudFormation
```js
{
    "Resources": {
        "s3bucket": {
            "Type": "AWS::S3::Bucket",
            "Properties": {
                "BucketName": "bucket-name"
            }
        }
    }
}
```