# PoC_on_TFRecords
## Tensorflow Records- tf-records

```tf-records:```

- TFRecords is a tensorflow framework binary storage format which stores sequence of binary records.
- Sequency of binar records means we need to create a data structure(name,values) manually to store the data in binary format.
- TFRecords,Internally uses protocol buffer to serialize the structure data. Also helps to create a communication between two interface via wire or store the data.

***Advantages of using tf-records:***
- When we are working on large dataset, using binary file format for storage it may have significant impact in terms of performance on our data pipeline and required training time of your machine learning model.
- Huge data we can store in less memory space though it's a binary file format.
- Binary data takes less time to copy,read and load the data from the disk.
- Easy to combine multiple data sources to **.tfrecord.** 
- More optimized version of lighter xml.

***Dis-advantages of using tf-records:***
- You have to convert your data to this format in the first place and only limited documentation is available on how to do that.
- Since, It store's in sequence format we need to create data structure manually with name and values which is very pain task if you are dealing with large table columns.
## Structuring TFRecords
- A TFRecord file stores your data as a sequence of binary strings. This means you need to specify the structure of your data before you write it to the file.
- Tensorflow provides two ways to structure the the data

1) ***tf.train.Example***

2) ***tf.train.SequenceExample.***
